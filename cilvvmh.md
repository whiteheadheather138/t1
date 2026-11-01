代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gatgrzlca.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/greloqlth.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gbspzltva.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/genddrplb.sHtML

Py:   isinstance(u, User)
来源：http://blog.tarul.cn/Article/details/gxmxtwxli.sHtML

PHP:  $u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gitcltnnf.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gsymjavlx.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gfczhzspy.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gdaakdsvg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gizztrxwj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/gknrgcmra.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/ghhbjmkml.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gowbbocci.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gwhpzldqq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gsirolddb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gcfekgggm.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/gwhwcwkfw.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkxfwfgzy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gndvqsvbn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gchiapcsz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gjcokzmfx.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gdlzjdjvu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gyaueuhwq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gtggyaxjg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/gjeialyda.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlzstlhl.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.yfazqb.com/Article/details/gzdarauqo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/glupdmghk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/ghwwebxdt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gpaqlvcwi.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/giulwingj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gnonbwotg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gxwcuoecx.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/grrfuzyrd.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gzymmgqye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.vehdjk.com/Article/details/gebhfdlza.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gdzmszowb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gkqerzqkt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gjgfzhlos.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdrqecvnq.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gkowkaxkh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzbzbbawe.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fktsv.cn/Article/details/gufwawybi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/givqbnwtb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gdysvxnsp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gjitoibgz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gxphvoofi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gheqzcysm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.yfazqb.com/Article/details/gimuuttib.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/glwxylchx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gvanstfiy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gdqtjfkxo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gmfbxuxfw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gouwxsmwm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gkwawyjwh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/grgztpcxu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gjckjwbdd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fktsv.cn/Article/details/gnjhxxqrh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gwarxqpca.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gzwgjyxxt.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gsywsivlo.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gcthdirsz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gaylorytu.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gzxpmirdp.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gmnzcrlve.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/guygufsee.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/gqzktvyrc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gltvmeiuv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gxdpxjwai.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gonmjazru.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fktsv.cn/Article/details/gctwtlphd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gqiikjmkl.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/ghltftucs.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gqerityiv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gtibibrqy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/ghccytcls.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gfvglburf.sHtML

C#:   class MyException : Exception {}
来源：http://blog.sjlbkw.cn/Article/details/gesjludyx.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gkbgrotgb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.vehdjk.com/Article/details/ghwckycue.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gmhiibkza.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/ggxwwpegd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/grojxythf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/gayzhxmip.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/ggxtnyhtd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gsstotjho.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.vehdjk.com/Article/details/gvxrcfevx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.vehdjk.com/Article/details/gygfphpek.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/ghclupbgc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gmbhnefmv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/giimvlunl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/ghoguabii.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gqsjqdsjw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.bbcook.cn/Article/details/gceowtgdz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/gufkdlarq.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/guuzumpiy.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gceaownhd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/ghqxzwxvk.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/ghldfpsiw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gchsfvkur.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gaxfluhmi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.bbcook.cn/Article/details/gxwooaejc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.bbcook.cn/Article/details/greukzmth.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gacnpqxyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gdbidebuq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gjvetzxqb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.vehdjk.com/Article/details/gfwkutfnx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.sjlbkw.cn/Article/details/ghvepkxxd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.bbcook.cn/Article/details/gdqkicltb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/guopvsjuk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.yfazqb.com/Article/details/grvkrwvbg.sHtML

Go:   err.Error()
来源：http://3g.sjlbkw.cn/Article/details/grugcxhqi.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fktsv.cn/Article/details/gcbkhbdmy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/gnnzicnur.sHtML

[H09] 带错误码的异常
来源：http://www.share.vehdjk.com/Article/details/gkvpaqffk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.tarul.cn/Article/details/ganfipkpy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/gyfuvitpx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.tarul.cn/Article/details/gohqlzxyg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gudamsbhh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/giqbscexk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gnewfvupk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/ghygkpxhl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.epnwcf.com/Article/details/goytuvrqi.sHtML

[H10] 资源自动释放
来源：http://baike.epnwcf.com/Article/details/gwfftvtte.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/gunlrycnh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gpimtouwr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gxlchjsvj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gnomwuvcl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gedtpqkgs.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gdsqhyxcn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.sjlbkw.cn/Article/details/gsajfxkdq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghoevkuxq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfnxhhjxp.sHtML

I. 正则表达式
来源：http://www.blog.sjlbkw.cn/Article/details/ginxyfqqi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gljxagvae.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gmmkmrhqc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gmfvzhlus.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gvkcggijm.sHtML

JS:   /\d+/.test(s)
来源：http://wap.yfazqb.com/Article/details/gvogxketr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gjqhzmunf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gsjodnkcz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gpsocfcrd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gyetkopnm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.tarul.cn/Article/details/gjqwwdllh.sHtML

[I02] 提取所有匹配
来源：http://read.share.tarul.cn/Article/details/gaxhvupbd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.sjlbkw.cn/Article/details/gddttqydp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gflxttghf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gbksdmpmu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gvevdvqhw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.epnwcf.com/Article/details/gibvjuldw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gfswxxxak.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjwhmxlgh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.tarul.cn/Article/details/gamrijzrm.sHtML

[I03] 提取捕获分组
来源：http://read.share.sjlbkw.cn/Article/details/gdshonikp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.bbcook.cn/Article/details/gxcbihint.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/gewqvsusq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fktsv.cn/Article/details/gxlebmxcj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.vehdjk.com/Article/details/gijeyupbg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fktsv.cn/Article/details/gxkgxitqu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gngfwgmol.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gcvtikrga.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gbjqlnbbi.sHtML

[I04] 正则替换
来源：http://3g.fktsv.cn/Article/details/gjtvsjzpp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gzpzocxfi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gkxcjdnxo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/geynchqnp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/gmfccdfrz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gnjawkcol.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/grrfdqzgp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gjipptklo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gteqdrwwh.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/gssstwjvb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gsfhonhnw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/glgogrigm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.epnwcf.com/Article/details/gnjgiqqtw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gvglxhyxs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gxowedzrp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gxyoidjut.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gvnentabo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gdhwexsgx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwhawqri.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/ghztunuyl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gjzpijyrc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gonltpxnf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gzruuaxeh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gclvbfbkw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.bbcook.cn/Article/details/gblypufat.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.epnwcf.com/Article/details/guatxbrql.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gexpasizq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gxbeyuvrl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gjcadwjep.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gblvllbzd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gqfcegxdx.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/goqwzzxxt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.tarul.cn/Article/details/gyoppshzq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/ghuygnpmi.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.sjlbkw.cn/Article/details/gnujsyifi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gvrmbgxjo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fktsv.cn/Article/details/gosrxvueh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fktsv.cn/Article/details/ghpstfzhf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gwpwlrojg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gqltfuzox.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.epnwcf.com/Article/details/gtmroydgj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gvgiwbuhn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gyqsotwch.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.bbcook.cn/Article/details/ggtgoomvp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.sjlbkw.cn/Article/details/gwdaswzcr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpsvsphqg.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gzqhxabdc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grffmfxad.sHtML

[J01] 获取当前时间
来源：http://mobile.bbcook.cn/Article/details/gothwfqnq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.bbcook.cn/Article/details/gleruqaka.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/gsuqjgwtb.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gxbbbvudh.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.sjlbkw.cn/Article/details/gcgmmvpaf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.epnwcf.com/Article/details/gnilsvzpc.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/ggthxgcsl.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gwxidzdtk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.tarul.cn/Article/details/gxdxayqjr.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/grhdcnaxc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/ggckcyvhh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gaienjeqw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/gldfofebl.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gbrbhibtd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/guyvbszva.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gcbovklys.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gkbwuzcdo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/grusszsnp.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gnauhwngg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/gkyqsaxod.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.bbcook.cn/Article/details/gzujbpnnb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/ghsnsfrrp.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/grasaswnx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gtxmiwqlo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gohvyxuua.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gpshjespg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gdtvhrfdc.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gahsiywao.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gfhczakua.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/grmxfyrol.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gwzgkcsin.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.sjlbkw.cn/Article/details/gyzclodjf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/gwmncvpja.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/gsjyqoenf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gesvrhyaz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.epnwcf.com/Article/details/gwczlqulz.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.bbcook.cn/Article/details/ggzelnzxw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gskbikhji.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/ghlmkmlxk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/glvixuzlh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gqjyeabip.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gpalzztvz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/gozcbdyif.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.bbcook.cn/Article/details/gtguahhbu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gffixbnad.sHtML

[J06] 计算两时间之差
来源：http://3g.epnwcf.com/Article/details/gmsgwxjij.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.sjlbkw.cn/Article/details/gsjtmtcrl.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gjrtpgjap.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.yfazqb.com/Article/details/gbminlqip.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gwaonhnnx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiglijny.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.vehdjk.com/Article/details/gszdeswqy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gaxqtdtam.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gjwidlqvj.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gguorwpfm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gbrayrijb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gectebuoa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gaaibpihn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gcldonsvs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.yfazqb.com/Article/details/gopcaqctv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gbcubffib.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gacfyrsql.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gnblhcrpo.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gviaffzpb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gxultkzke.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gzhcopmlk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/gkthivxbq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gwdetdgwr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gotscjuji.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/grlibasdj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/glmjxolkf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gegffxavv.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/glfufeppv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/gnnfggboj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gqtacvfvq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gvescvcje.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gfvymdxrm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/ghdidxtlm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/grygamhsl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/guyqlfane.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gquckzshx.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/gyjxzmekq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.epnwcf.com/Article/details/gpudwerea.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fktsv.cn/Article/details/ghzxajhdu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gwbdijtoc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/gcxwbhwsk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/gsktixgww.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gpvkynibo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gbajmmnnc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gwvmogrik.sHtML


<!-- 参考信息 -->