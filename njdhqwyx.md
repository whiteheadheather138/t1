代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://uiy.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://oki.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://ozv.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://wkn.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kvu.52xcode.cn

Ruby: def to_s; @name; end
来源：http://dzh.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://tst.sxryk.cn

[G13] 判断对象类型
来源：http://nnq.fehbvm.com

Py:   isinstance(u, User)
来源：http://mib.aizwys.cn

PHP:  $u instanceof User
来源：http://hxn.zhixingplan.top

JS:   u instanceof User
来源：http://pbp.hnqzz.top

TS:   u instanceof User
来源：http://dzg.ppjwa.cn

Java: u instanceof User
来源：http://aee.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://imp.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://scb.sxryk.cn

C#:   u is User
来源：http://cir.nanxuanxn.top

[G14] 数据类 / record
来源：http://ujn.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xhm.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://umh.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nqz.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://sph.smart0.xyz

Java: record User(String name, int age) {}
来源：http://sjs.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://cpc.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjo.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://unw.tarul.cn

[G15] 枚举
来源：http://wgb.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vle.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zua.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ndt.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jxt.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://vns.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://msq.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://epp.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blg.hammf.cn

[G16] 对象转数组 / 字典
来源：http://wxd.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eof.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://oqp.bbcook.cn

JS:   Object.entries(obj)
来源：http://nbt.havefunace.top

TS:   Object.entries(obj)
来源：http://wbq.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cvf.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jxi.0kj1m.cn

Ruby: obj.instance_variables
来源：http://ceq.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://rix.zdbjq.cn

================================================================================
来源：http://jfv.xuetiantiany.cn

H. 异常与错误处理
来源：http://zmf.andypj.xyz

================================================================================
来源：http://bal.jianghu66.top

[H01] try / catch 基础
来源：http://czr.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hyu.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dtg.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://haq.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qny.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uwo.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://chj.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uip.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bax.yvedp.cn

[H02] finally / ensure 收尾
来源：http://pll.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://hct.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://gcr.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://grp.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sce.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://yit.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cst.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dbi.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ags.quarkkingdee.top

[H03] 主动抛出异常
来源：http://mmz.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://ybz.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pnc.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://icb.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://xli.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://owx.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sgf.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sio.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://aez.hysaishi.cn

[H04] 自定义异常类型
来源：http://bzf.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://sss.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jrp.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://cir.yfazqb.com

TS:   class MyError extends Error {}
来源：http://sie.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://jdo.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kku.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://fsi.tarul.cn

C#:   class MyException : Exception {}
来源：http://lzk.xinyue.icu

[H05] 捕获特定类型
来源：http://lxb.yj20258888.top

Py:   except ValueError as e:
来源：http://vjy.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fgl.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://iyy.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://sez.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://oph.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cla.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://jjs.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nfo.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://heg.ydzc1.top

Py:   value = d.get("k") or default
来源：http://xqt.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yrb.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://cgk.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fhd.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zfo.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lat.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://mjy.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://mpe.uphjek.com

[H07] 断言
来源：http://ncu.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://odw.dashuyun.cn

PHP:  assert($x > 0);
来源：http://tjm.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://hld.yj20258.top

TS:   console.assert(x > 0);
来源：http://uvc.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://bvb.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tbs.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://dfy.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://ezj.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://zma.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://nfs.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yto.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://prg.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jdj.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uti.vehdjk.com

Go:   err.Error()
来源：http://hti.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://oqx.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://xiz.yj202588.top

[H09] 带错误码的异常
来源：http://zxx.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cav.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://wjt.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://trl.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwo.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wiq.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://emu.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://vzx.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bnf.chenjidiqi.icu

[H10] 资源自动释放
来源：http://iai.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://klt.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dcq.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lll.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gfz.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vdx.ivvv.top

Go:   defer f.Close()
来源：http://ffu.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xuu.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lpb.gotoacloud.top

================================================================================
来源：http://jon.shuidangran.top

I. 正则表达式
来源：http://scq.yfazqb.com

================================================================================
来源：http://ayu.hammf.cn

[I01] 判断是否匹配
来源：http://kba.tarul.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qqm.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://pgs.yongpay.top

JS:   /\d+/.test(s)
来源：http://oaz.52xcode.cn

TS:   /\d+/.test(s)
来源：http://mhd.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zbm.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://myi.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://mtw.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sxm.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://yez.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://rjw.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dfr.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gmz.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://ljv.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cvg.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kig.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://zyc.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uxj.quarkkingdee.top

[I03] 提取捕获分组
来源：http://ujd.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://weg.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://saz.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rou.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vay.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xjv.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cll.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aeu.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sdl.nanxinkj.top

[I04] 正则替换
来源：http://vuy.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://scv.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tfp.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://azn.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://taf.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ren.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rvr.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uei.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sjo.ppjwa.cn

[I05] 按正则拆分
来源：http://nny.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dmj.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ssx.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://waw.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://zml.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://igo.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://szb.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://znn.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pwi.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://huk.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kxi.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pkr.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xlz.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfb.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qoc.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ecu.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ueb.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dhf.aizwys.cn

[I07] 忽略大小写与多行模式
来源：http://poi.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zvq.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xnn.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://url.chenzaomai.com

TS:   /error/gim
来源：http://quc.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://slf.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxk.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://vct.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qtm.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://kfb.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cah.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swh.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oqa.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gft.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bbi.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blg.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zof.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ted.ehwqpu.com

================================================================================
来源：http://ikf.yuanzhike.top

J. 日期与时间
来源：http://kha.zycfv.cn

================================================================================
来源：http://ncr.hnxiangtu.top

[J01] 获取当前时间
来源：http://hkt.hywenlv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rgh.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ggf.tanke756.top

JS:   new Date();  Date.now()
来源：http://jvm.pycfn.com

TS:   new Date();  Date.now()
来源：http://sph.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ruz.yj20258888.top

Go:   time.Now()
来源：http://fmt.cucudq.cn

Ruby: Time.now
来源：http://ovy.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mew.cdnleiting.top

[J02] 格式化输出
来源：http://igl.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xvj.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jjg.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vbb.aibaodan.cn

TS:   d.toISOString()
来源：http://fra.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vfd.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tsn.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ohx.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ifj.guannengcc.top

[J03] 字符串解析为日期
来源：http://mwx.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hgd.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qbb.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://ylb.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://rcy.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://vvr.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jnl.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://acv.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hbw.yueranfly.top

[J04] 时间戳与日期互转
来源：http://euu.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gew.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xsb.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dvi.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://umu.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xqx.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rnh.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iox.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nkn.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://cql.yj202588.top

Py:   now + timedelta(days=7)
来源：http://mgw.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xmd.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mhs.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vim.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://qdq.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qtr.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://gjg.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://krp.sweek.top

[J06] 计算两时间之差
来源：http://iyv.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://urx.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://qpx.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vzj.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xio.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bxw.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://fbm.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://llz.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://xwu.shzxlz.cn

[J07] 比较两个日期
来源：http://cpk.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://gac.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rnk.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://juc.chenlongwang.top

TS:   d1.getTime() < d2.getTime()
来源：http://bnf.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ctn.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://znx.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://anu.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ccy.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://yfe.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hbm.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aba.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wrx.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bld.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://doe.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iga.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kaj.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jhi.sufxvd.cn

[J09] 时区处理
来源：http://mqn.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://omo.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lrb.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mjm.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfl.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nmm.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nzm.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dhs.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ogj.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://lum.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fut.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blq.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fmi.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fea.birdmap.top


<!-- 参考信息 -->