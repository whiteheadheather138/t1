代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://pzb.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://hvq.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://bys.sjlbkw.cn

[G13] 判断对象类型
来源：http://dbb.yfazqb.com

Py:   isinstance(u, User)
来源：http://qui.zhongyouzk.top

PHP:  $u instanceof User
来源：http://seo.jianghu66.top

JS:   u instanceof User
来源：http://ytx.sweek.top

TS:   u instanceof User
来源：http://atr.hongshengwenyu.top

Java: u instanceof User
来源：http://kbd.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kmb.cashguo.top

Ruby: u.is_a?(User)
来源：http://fvk.chenjidiqi.icu

C#:   u is User
来源：http://axy.xuanzx.com

[G14] 数据类 / record
来源：http://nbh.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ahq.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://pbr.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://mjc.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://scg.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://nox.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://fav.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tuu.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://zwd.hysaishi.cn

[G15] 枚举
来源：http://dxk.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://opv.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ick.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyd.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bzu.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://vvd.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bqu.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://vxk.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ucw.uphjek.com

[G16] 对象转数组 / 字典
来源：http://bem.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yol.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://mhs.yueranfly.top

JS:   Object.entries(obj)
来源：http://eyb.yueranfly.top

TS:   Object.entries(obj)
来源：http://tbp.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gyy.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://aiw.yuanzhike.top

Ruby: obj.instance_variables
来源：http://ypn.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://qyl.bjfxy.top

================================================================================
来源：http://uws.pengpengdd.cyou

H. 异常与错误处理
来源：http://syz.zhengqikj.top

================================================================================
来源：http://ubm.c1oappe.top

[H01] try / catch 基础
来源：http://afw.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bbw.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gyi.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bxp.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://moe.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dym.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aky.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bvp.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pqo.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://xkd.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fua.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dbh.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ilx.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pxa.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://vuu.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yoq.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qor.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jhm.cucudq.cn

[H03] 主动抛出异常
来源：http://fbu.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://css.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://owd.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://zir.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://cmy.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qfa.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gge.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hrz.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gpv.aizwys.cn

[H04] 自定义异常类型
来源：http://lcb.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://vcj.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://zdq.xuanzx.com

JS:   class MyError extends Error {}
来源：http://jle.yuxming.cn

TS:   class MyError extends Error {}
来源：http://xxv.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://kvv.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ydd.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://syt.fengsongda.top

C#:   class MyException : Exception {}
来源：http://suj.daria6918.cn

[H05] 捕获特定类型
来源：http://gfu.shuidangran.top

Py:   except ValueError as e:
来源：http://jgk.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mlg.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://iyt.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://waz.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://ugt.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rbx.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://bib.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tgk.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://rcu.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://cbl.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://yqu.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hmt.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://aac.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cwg.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dev.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://vbb.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://wwo.hfpthk.cn

[H07] 断言
来源：http://gge.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://uao.havefunace.top

PHP:  assert($x > 0);
来源：http://axz.fengsongda.top

JS:   console.assert(x > 0);
来源：http://ndc.ybcxt.top

TS:   console.assert(x > 0);
来源：http://xzv.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://trs.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wbf.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uix.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://sso.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://uqa.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://hln.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpx.hesvh.cn

JS:   e.message;  e.stack
来源：http://kqt.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://twc.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zew.jinyuanbaomall.cn

Go:   err.Error()
来源：http://unr.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://asg.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://zxb.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://xot.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lzs.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sxg.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vyg.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xkh.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rec.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://txe.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://xsn.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lnn.zhengqikj.top

[H10] 资源自动释放
来源：http://dku.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://upf.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pwb.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zqq.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fyi.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pwu.fengsongda.top

Go:   defer f.Close()
来源：http://xbe.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vko.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://owl.iojbl.cn

================================================================================
来源：http://jas.dianchejie.cn

I. 正则表达式
来源：http://gyz.316326.xyz

================================================================================
来源：http://wxu.uphjek.com

[I01] 判断是否匹配
来源：http://puk.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blw.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://nmz.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://eiu.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://jmg.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mir.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rnh.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://mll.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xvl.fktsv.cn

[I02] 提取所有匹配
来源：http://yto.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://jch.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wxd.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vyp.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://wfv.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tpp.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xso.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://jlv.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mqw.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://tut.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dek.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://req.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kya.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xxl.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gnx.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://swo.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sbc.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rsf.shanyushiyangtech.top

[I04] 正则替换
来源：http://zpq.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://gkg.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gew.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://wbc.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://rbx.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://jxp.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://owl.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ylr.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sif.zhengqikj.top

[I05] 按正则拆分
来源：http://gqw.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://sdx.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dkb.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://gfc.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://foy.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://cvn.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jxz.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://ugv.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gav.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://atg.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dvz.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xiq.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kup.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdn.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://giw.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ops.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tbk.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gwh.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://mmu.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bho.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qne.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vjw.pengpengdd.cyou

TS:   /error/gim
来源：http://mbq.nanxinkj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zzm.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bfy.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://yro.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://htp.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://zli.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zsd.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rxp.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oue.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oup.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hdo.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xoh.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bdn.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yvd.xuetiantiany.cn

================================================================================
来源：http://bfr.hnqzz.top

J. 日期与时间
来源：http://ujd.jinqigufen.top

================================================================================
来源：http://mxn.fehbvm.com

[J01] 获取当前时间
来源：http://ijy.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iwe.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jeq.xziqi.cn

JS:   new Date();  Date.now()
来源：http://inp.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://ruy.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://mdz.316326.xyz

Go:   time.Now()
来源：http://ltb.daria6918.cn

Ruby: Time.now
来源：http://egk.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oyk.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://gpq.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gsi.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://acz.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xjg.sjlbkw.cn

TS:   d.toISOString()
来源：http://mpt.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://svz.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://txh.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://agc.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cgk.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://rum.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cyr.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dcv.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://swr.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://miq.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cpo.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nkt.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://mzl.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vzd.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://wvt.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bsf.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ith.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hvy.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jhr.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://skz.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xdf.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbs.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ask.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://ykx.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://gig.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sit.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hyk.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://seh.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://uvi.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wtd.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://kxj.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://vmg.xuanzx.com

[J06] 计算两时间之差
来源：http://uhg.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://ren.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://cbe.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ijs.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://chk.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hjm.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://bia.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://wxc.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://dgi.chenzaomai.com

[J07] 比较两个日期
来源：http://uyd.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://hov.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qae.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://dyv.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://jge.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fsb.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zcb.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ulp.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://ehm.hcnkem.com

[J08] 提取年月日与星期
来源：http://ptr.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hdo.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qyv.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dpx.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://crv.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tum.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxe.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qmq.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gdw.sxryk.cn

[J09] 时区处理
来源：http://guq.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vbf.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pzp.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xce.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://let.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mjl.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://egr.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qku.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cpr.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://wwb.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://jtb.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mhb.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jex.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://txi.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://atm.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ect.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nzb.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://huk.fehbvm.com


<!-- 参考信息 -->