require 'asciidoctor'

guard 'shell' do
  watch(/^dev-tools\.adoc$/) {|m|
    Asciidoctor.convert_file m[0], to_file: true, safe: :safe
  }
end

guard 'livereload' do
  watch(%r{^.+\.(css|js|html)$})
end
