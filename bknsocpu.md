代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://lwe.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://yuh.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://mdl.cheryme.top

[G13] 判断对象类型
来源：http://fmz.hnqzz.top

Py:   isinstance(u, User)
来源：http://oze.mhx1999.top

PHP:  $u instanceof User
来源：http://luh.cdnleiting.top

JS:   u instanceof User
来源：http://kxr.bbcook.cn

TS:   u instanceof User
来源：http://glp.yangfankeji.com

Java: u instanceof User
来源：http://gdt.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://meg.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://cxw.shanyushiyangkeji.top

C#:   u is User
来源：http://mqf.zhoulong.xyz

[G14] 数据类 / record
来源：http://abk.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cvl.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://fsr.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://ush.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://zfp.ivvv.top

Java: record User(String name, int age) {}
来源：http://pcj.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://nfu.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tcy.cashguo.top

C#:   record User(string Name, int Age);
来源：http://nda.yfazqb.com

[G15] 枚举
来源：http://aoq.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ytr.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://vzw.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://phd.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ppd.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://biy.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqx.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://eql.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://seo.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://xft.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://myv.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://rjj.jinqigufen.top

JS:   Object.entries(obj)
来源：http://xyy.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://yvd.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nrc.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://srr.yvedp.cn

Ruby: obj.instance_variables
来源：http://vbx.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://eqr.chenlongwang.top

================================================================================
来源：http://seg.jlsjyb.cn

H. 异常与错误处理
来源：http://whd.andypj.xyz

================================================================================
来源：http://sdt.snrcjt.cn

[H01] try / catch 基础
来源：http://iqa.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oaa.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wyg.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vyb.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tpv.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://awa.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zjf.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rlo.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hir.ybcxt.top

[H02] finally / ensure 收尾
来源：http://cld.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://jaj.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kww.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lpq.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hik.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://ody.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gxo.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://trk.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ald.jqgufenzy.top

[H03] 主动抛出异常
来源：http://sfx.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://dob.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bfb.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://yck.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://pnr.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sbo.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bry.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://daj.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gry.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://sat.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://vjm.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://zgg.mhx1999.top

JS:   class MyError extends Error {}
来源：http://qyv.havefunace.top

TS:   class MyError extends Error {}
来源：http://dem.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://bkk.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ufx.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://bsi.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://tld.nwbrower.top

[H05] 捕获特定类型
来源：http://hzl.yj20258.top

Py:   except ValueError as e:
来源：http://xtm.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://egy.pengpengdd.cyou

JS:   if (e instanceof TypeError) {}
来源：http://tgz.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://cln.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://fqd.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vfy.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://bfi.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hxz.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://lad.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://bja.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nto.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eyl.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hcf.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fsa.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://orc.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://nxt.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://rkz.daxiang520.top

[H07] 断言
来源：http://lmt.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://ywy.gogol.net.cn

PHP:  assert($x > 0);
来源：http://rxy.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://brb.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://sld.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://azp.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://skp.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nhv.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://dts.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://mlt.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ofo.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aeq.mhx1999.top

JS:   e.message;  e.stack
来源：http://lip.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aay.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hnc.jqgfzy.top

Go:   err.Error()
来源：http://uwe.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://dbg.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://bdt.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://itq.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://noo.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wtm.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://woc.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gdr.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rjv.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://usm.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gxq.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://llz.fktsv.cn

[H10] 资源自动释放
来源：http://vhs.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wes.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ynd.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lzv.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://swq.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ows.zhengqikj.top

Go:   defer f.Close()
来源：http://nck.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mol.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vxu.yangfankeji.com

================================================================================
来源：http://txl.pycfn.com

I. 正则表达式
来源：http://shx.xuanzx.com

================================================================================
来源：http://xnx.ybcxt.top

[I01] 判断是否匹配
来源：http://ofu.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sbh.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nur.jianghu66.top

JS:   /\d+/.test(s)
来源：http://mox.guannengcc.top

TS:   /\d+/.test(s)
来源：http://azj.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dso.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fxl.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://lqu.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dmz.zhoulong.xyz

[I02] 提取所有匹配
来源：http://nxd.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://tzq.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aaj.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vpb.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://qvr.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zfu.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rsv.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://iqh.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yon.c1oappe.top

[I03] 提取捕获分组
来源：http://vyp.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jzl.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hqb.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ufk.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bfc.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zuz.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eup.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pdv.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nvc.sweek.top

[I04] 正则替换
来源：http://twk.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iin.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jwp.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://qqo.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gom.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hon.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ace.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qgj.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uxd.smart0.xyz

[I05] 按正则拆分
来源：http://siz.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uxw.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vzh.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://rnl.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://zqf.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://icu.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kzf.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://irk.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ntg.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ksm.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ako.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lid.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gwm.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ndd.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jjp.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://giy.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dzm.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://phd.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://eti.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qfh.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vhr.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pnp.pycfn.com

TS:   /error/gim
来源：http://pff.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xvt.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ylt.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://roh.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxn.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://ohh.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tcf.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wsh.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aed.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqy.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://hhq.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ams.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ama.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ixk.chenlongwang.top

================================================================================
来源：http://bpo.epnwcf.com

J. 日期与时间
来源：http://cnu.hnxiangtu.top

================================================================================
来源：http://qgz.zdbjq.cn

[J01] 获取当前时间
来源：http://epj.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bik.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qvy.ybcxt.top

JS:   new Date();  Date.now()
来源：http://yyf.yueranfly.top

TS:   new Date();  Date.now()
来源：http://yjn.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dwr.yongpay.top

Go:   time.Now()
来源：http://jlj.xuanzx.com

Ruby: Time.now
来源：http://pov.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ufi.ydjk.org.cn

[J02] 格式化输出
来源：http://etx.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mhg.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rzg.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wrc.bbcook.cn

TS:   d.toISOString()
来源：http://bkm.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xrv.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://moo.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pku.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://duw.yj20258888.top

[J03] 字符串解析为日期
来源：http://lyw.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jna.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ahv.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://tit.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://zdp.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://pux.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pai.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://nbu.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lez.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://bfj.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qjt.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uih.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zla.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ltm.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rvh.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xgi.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sgr.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bgm.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://bnm.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://fnz.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hyv.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kft.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rqb.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://trt.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fdo.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://oht.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eww.uphjek.com

[J06] 计算两时间之差
来源：http://kcb.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://rlb.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://imk.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ktm.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://txf.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://zpx.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://izm.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://weo.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://jin.yfazqb.com

[J07] 比较两个日期
来源：http://gym.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://wnp.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://myy.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ujo.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://yjz.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ljx.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kzh.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jmh.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://kqj.316326.xyz

[J08] 提取年月日与星期
来源：http://rha.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fds.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mnw.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bon.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pvx.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eks.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mgc.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zne.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lrk.ctjpmb.com

[J09] 时区处理
来源：http://uue.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qyc.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://owo.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbb.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cse.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blb.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eun.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fuo.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jmj.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://rgb.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qxd.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tvy.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fwl.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nnh.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jli.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qog.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ocv.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tdz.hongshengwenyu.top


<!-- 参考信息 -->