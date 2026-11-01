代发 wailian999

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gvpuxjbov.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gvyuritmj.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/ggamgroqh.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gqmogxylv.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gzkhevwkc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gomqtvziu.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gyiokkqvi.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/gvbkbewuf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gxalntnha.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gnpdzrsqr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/glxiebvme.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gekccohno.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gkjjgcvmu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gqeqtslcy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/ghumorbfu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gcmftzsku.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gnfpxjysf.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gmrmyojjz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.epnwcf.com/Article/details/gilxydwsl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdgbnotw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/gnjrmypqt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gakhgbtuj.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fktsv.cn/Article/details/geybdijap.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/gjyuqwbbm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gdrnjbogn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gaalzncov.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/ggzroirfc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gwzjwwvkx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gwounodfq.sHtML

JS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gxhfpecln.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gukmxhxpn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/glhofvpox.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.tarul.cn/Article/details/gvjptoljd.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/gscrmcyxx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/geayfkdto.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvzbvjizk.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gsddperib.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gprnwzrdj.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/gqtcxskfb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gthncxexe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/giakbsxvp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/ggwuontpu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gwodtrmgt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/gglqkqgkj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.epnwcf.com/Article/details/gqrwzfdma.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/ghzbexbkn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/ghahocsyj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fktsv.cn/Article/details/gohaxefej.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gyggtvklb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/ghtffrdmp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gouuyvhox.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gkfdaezil.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gplediwux.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.epnwcf.com/Article/details/gulgagyib.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gzsesgyrz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gnakzqfat.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwyreccx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/gqevtdkkl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gedxawuou.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gottuiysz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gnfcycvjb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gsmcuvzko.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fktsv.cn/Article/details/ghwjdvxxk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.bbcook.cn/Article/details/geqwzayim.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/glujazgvr.sHtML

[H04] 自定义异常类型
来源：http://www.share.yfazqb.com/Article/details/guplwzyht.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gskbtiztw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gvplbifwx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gwyxdyhsw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gzxlonltj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gbpbjtzqm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gtuatfdjn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fktsv.cn/Article/details/gijoharcf.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/gkfpagbwu.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gyrmnxpao.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gmgrhbwsx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gjqokuhpf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/ghbmedmfy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gepabhnjq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gkrgsodtk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.tarul.cn/Article/details/gboyaraec.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gnrzpcpek.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gtulwtnee.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.vehdjk.com/Article/details/grlrcxbhz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/getauvgjg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gtzuzltig.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gyzfyohpt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gobuomyyc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/gmzljtcta.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gexpccros.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gqkvfwfjz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.tarul.cn/Article/details/gdjjueyix.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gfybbhuqq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/gdxgvbuya.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/gojwryfdn.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/glzwdqpuc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gqscoxpdw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.epnwcf.com/Article/details/gwmtfgbfj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gyzhpgful.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.tarul.cn/Article/details/gtmwwpltw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gvztkcpni.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcrkrfvd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.yfazqb.com/Article/details/gtoksifgv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gfyzzaoly.sHtML

JS:   e.message;  e.stack
来源：http://read.share.vehdjk.com/Article/details/gkkotxpps.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gtjxazrzk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.sjlbkw.cn/Article/details/gfjvgisag.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gircmbpxf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gtfkbjcfb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/gkxjljzgf.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/genuxglvo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/geghimxmd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gxdpdctpb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.vehdjk.com/Article/details/gisiltbdf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.bbcook.cn/Article/details/gtjwuowds.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.bbcook.cn/Article/details/gecouvets.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.epnwcf.com/Article/details/gpeaygttq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/guuznxmmv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gdsjjufwe.sHtML

[H10] 资源自动释放
来源：http://www.blog.sjlbkw.cn/Article/details/glgmjztwy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fktsv.cn/Article/details/gzcngzadf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqdtdxss.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gvfypivil.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/gcnmjjehj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fktsv.cn/Article/details/ggqciqbdd.sHtML

Go:   defer f.Close()
来源：http://www.blog.tarul.cn/Article/details/gdgtgzxny.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gqefxuxju.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gubdbmooc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gapkborcj.sHtML

I. 正则表达式
来源：http://wap.tarul.cn/Article/details/gucucwphw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdsvswfjb.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gzsqczvin.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gvhilakay.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gtuftvqro.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxlyxyicq.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.bbcook.cn/Article/details/gyxfcuwku.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.bbcook.cn/Article/details/gnzmcojjq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/giwtjljiz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/grlazdytf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gzkwjtwid.sHtML

[I02] 提取所有匹配
来源：http://www.blog.yfazqb.com/Article/details/gpjuuovmm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gxpmmxand.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gwaovpmtb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gefjqeaxn.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gncgwoxrn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.bbcook.cn/Article/details/gqhyzqyri.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gomimekiw.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/glysjevon.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.tarul.cn/Article/details/gktxihvyr.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gdcsufxok.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzcizfeyz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/gapcznkxw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gljefxxxk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/goyeorlau.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/gleemjoio.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fktsv.cn/Article/details/gofyidooc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.yfazqb.com/Article/details/gajjqdxat.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.tarul.cn/Article/details/grhfbdszy.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/gjwkxcgcx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.tarul.cn/Article/details/gywubstlj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gmzfaubif.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gtcekptfv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzbtwvzq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gdlvtexbk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/gacxizwmu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.bbcook.cn/Article/details/guvvkyfox.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fktsv.cn/Article/details/gtnxvtqax.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gzhcnvrqm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.epnwcf.com/Article/details/gmeubljls.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/godcstorm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/geoepkkhn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gflzdiqpk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.tarul.cn/Article/details/gxztmokdt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gxnaczgtx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gidbmxhdp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/gzsuencbd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gmbqrrymg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/ghpzhdxvd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gyhlhgbfu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gingkdonf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gcmgdbisi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.tarul.cn/Article/details/gdqspfvzb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.sjlbkw.cn/Article/details/gzywxdewg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fktsv.cn/Article/details/gjcbojobz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gwmnyptez.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/gyxoayuzt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.yfazqb.com/Article/details/gfkatbpxz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gtaumwpoe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/gusavdivv.sHtML

TS:   /error/gim
来源：http://m.share.bbcook.cn/Article/details/gpfxjdrvk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.vehdjk.com/Article/details/gonwlaotj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gwonrlqrw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.epnwcf.com/Article/details/gyrozvlmi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gnwzwhxsl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gxboaewqb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gmobigktv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.vehdjk.com/Article/details/gxdqomxio.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqhosxwu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gqwmzeyeq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gtjrnedry.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gqqxxkuvh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fktsv.cn/Article/details/gdgczdmzb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/ggkvdlvhs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxrmwzkar.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gvqigfvno.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxppqfbuh.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gwlcunnqn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/gxhuwokaz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gwodjanug.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gsxjdvtnr.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.vehdjk.com/Article/details/gswkbysaw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.yfazqb.com/Article/details/gmqhxwvuj.sHtML

Go:   time.Now()
来源：http://mobile.epnwcf.com/Article/details/gwnvqivyx.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gaeznstdi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gvxbkmbcz.sHtML

[J02] 格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gftwbndmd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gepsrhhve.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/gbztdaehf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gecsvyklq.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/ghraonbhk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/guusxuplq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.sjlbkw.cn/Article/details/gsftpkoan.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/giuodbdfr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.sjlbkw.cn/Article/details/gssjpmmjq.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/gvuvgycrz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gmzycgqyv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/gcmlfnjiu.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/giyapsdrj.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gsdrxcqni.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gbovlryct.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gcinmlfha.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gycxzbxtl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gcwurzwfr.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/ghfjpoxgu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.tarul.cn/Article/details/gbcxyyglj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gjswpkxgo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.bbcook.cn/Article/details/gmjkgxbhp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.sjlbkw.cn/Article/details/grbnrzkmp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gazjrlmcf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gyfstcgnz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggryionew.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gpzxvsoac.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gjmejgjrf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/gvergdjca.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gitmswdwy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gclzdmito.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gtkuhgxxt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gbsjbkunw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.bbcook.cn/Article/details/gqynedabl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gshundesz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gtywmfeco.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gmznbzbyw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gtpafuqcx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/gkpjmvolo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/ggylqrfzd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.tarul.cn/Article/details/gfwsqcwhw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fktsv.cn/Article/details/ggrptopso.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/gvwdukpqa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gklvygniz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/gtbaqmbam.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/gqkuotoho.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gmsslpsnc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.sjlbkw.cn/Article/details/gyhboxiyq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/ghvlfmgmb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gsmatquim.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fktsv.cn/Article/details/ggnxdxjwc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/glmkhnmkh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gnalqvqic.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gbzoxgrzk.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.sjlbkw.cn/Article/details/gmugutjrm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gdrabkvkf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gqjtxuyvs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gsvefdqwg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.tarul.cn/Article/details/ghsqhmygj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/ggiirnnli.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/ggbezuhoz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gcfoegeor.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gwcdefhib.sHtML

[J09] 时区处理
来源：http://m.share.sjlbkw.cn/Article/details/gcoueqynf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/gmeviyhxj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gyszbdfdn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gzdpfonwv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gttllgdqf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/gakhwzhwk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gcpomyycx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gjffwixli.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gonkmlyfr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/gbzlrosfi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gphrarmuj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/ghorcczsk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/gnkbrxqyp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/ghuquvpfr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.bbcook.cn/Article/details/gpnngzpob.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.yfazqb.com/Article/details/giaoiexsl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gfzqnpguf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/ghhjnldhd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gazldeoxe.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/geqzsesuw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzsldtoxc.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gbwihhfrh.sHtML


<!-- 参考信息 -->