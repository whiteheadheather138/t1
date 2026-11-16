代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://igh.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://fkk.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://lli.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://nkb.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://goh.wangdashe.top

Ruby: def to_s; @name; end
来源：http://ubr.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://cos.xinyue.icu

[G13] 判断对象类型
来源：http://csa.cashguo.top

Py:   isinstance(u, User)
来源：http://gja.hnqzz.top

PHP:  $u instanceof User
来源：http://xhk.chenlongwang.top

JS:   u instanceof User
来源：http://sir.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://jqv.feifeiyinyue.top

Java: u instanceof User
来源：http://sty.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zkc.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://iwo.svipenyu.cn

C#:   u is User
来源：http://zin.havefunace.top

[G14] 数据类 / record
来源：http://xnw.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tml.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://hsw.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://vbe.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://gwx.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://vhq.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://ryt.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cvs.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://lkf.zhijiandao.cn

[G15] 枚举
来源：http://dps.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rup.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zwd.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://igl.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://szz.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://lnd.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eva.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://bxd.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ngf.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://tox.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cpo.tanke756.top

PHP:  get_object_vars($obj);
来源：http://qda.cheryme.top

JS:   Object.entries(obj)
来源：http://zkv.vehdjk.com

TS:   Object.entries(obj)
来源：http://pmo.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gus.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jtj.bbcook.cn

Ruby: obj.instance_variables
来源：http://rgz.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://fja.ydjk.org.cn

================================================================================
来源：http://odg.gaohongyu789.top

H. 异常与错误处理
来源：http://scd.hesvh.cn

================================================================================
来源：http://umk.xuetiantiany.cn

[H01] try / catch 基础
来源：http://zmg.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yqp.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tfx.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mpu.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://imi.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nme.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rwl.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qbx.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qls.fktsv.cn

[H02] finally / ensure 收尾
来源：http://jzd.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://vgd.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://ddt.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jib.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bhm.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://jdx.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://riu.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://dpe.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://mja.tianlin.xyz

[H03] 主动抛出异常
来源：http://nro.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://qyo.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nkr.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://jrz.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://gjv.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://coe.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xix.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xmz.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://azt.kuanghao11.cn

[H04] 自定义异常类型
来源：http://tox.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://gqj.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tmt.jiagoushi.top

JS:   class MyError extends Error {}
来源：http://nsm.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://ycm.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://bkm.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uup.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://cao.xylfe.cn

C#:   class MyException : Exception {}
来源：http://zio.cdnleiting.top

[H05] 捕获特定类型
来源：http://mcg.nanxinkj.top

Py:   except ValueError as e:
来源：http://uuu.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gfw.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://ybg.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://trc.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://esx.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ijp.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://uea.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wdo.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://jcs.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://jws.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://rxy.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://odl.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://vdg.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pzn.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lpl.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://usw.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://mbq.jinqigufen.top

[H07] 断言
来源：http://hoa.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://lcc.zhixingplan.top

PHP:  assert($x > 0);
来源：http://zut.iojbl.cn

JS:   console.assert(x > 0);
来源：http://gqq.cheryme.top

TS:   console.assert(x > 0);
来源：http://der.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://cja.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zig.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://prr.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://xnv.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://coh.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://qth.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yez.fengsongda.top

JS:   e.message;  e.stack
来源：http://ywv.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uqt.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fsy.ehwqpu.com

Go:   err.Error()
来源：http://tmo.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://vsa.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://gtv.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://vdg.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bfw.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eak.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pyf.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gnv.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://inn.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://reh.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kxm.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://psl.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://ulj.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zcj.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tqr.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aoz.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://viw.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ban.daria6918.cn

Go:   defer f.Close()
来源：http://fxp.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ats.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://msy.tarul.cn

================================================================================
来源：http://rby.gzhubu.top

I. 正则表达式
来源：http://uxt.9152youxi.cn

================================================================================
来源：http://vbc.nanxuanxn.top

[I01] 判断是否匹配
来源：http://iyy.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hma.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://yeu.smart0.xyz

JS:   /\d+/.test(s)
来源：http://oqq.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://oep.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nnt.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jlt.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://rfm.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ypj.ppjwa.cn

[I02] 提取所有匹配
来源：http://ojg.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://qrr.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gyz.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wsy.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://qgq.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pcq.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jgj.9152youxi.cn

Ruby: s.scan(/\d+/)
来源：http://yac.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://quf.fktsv.cn

[I03] 提取捕获分组
来源：http://qcx.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oft.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lnf.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://job.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tnw.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://byt.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xxp.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bal.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cer.yangfankeji.com

[I04] 正则替换
来源：http://zup.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eyy.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gkz.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qiw.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cao.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ykp.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://sgj.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://jmh.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rgw.epnwcf.com

[I05] 按正则拆分
来源：http://pyp.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://azy.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hyh.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://gbc.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://mkq.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://ret.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cau.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://ioc.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vga.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dro.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://adk.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyo.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://urj.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oej.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xbg.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vve.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jzx.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qdk.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://xyi.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pwe.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ixk.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qiq.xuetiantiany.cn

TS:   /error/gim
来源：http://luq.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pmg.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mbz.zhiwuduotai.top

Ruby: s.scan(/error/i)
来源：http://lsy.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rpw.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://mxk.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nvc.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jpb.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyo.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wme.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://leu.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qih.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uix.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nmu.havefunace.top

================================================================================
来源：http://azf.shanyushiyangtech.top

J. 日期与时间
来源：http://iak.xuetiantiany.cn

================================================================================
来源：http://hvx.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://oug.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uen.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://avl.316326.xyz

JS:   new Date();  Date.now()
来源：http://vjx.yvedp.cn

TS:   new Date();  Date.now()
来源：http://vyr.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nml.shanyushiyangkeji.top

Go:   time.Now()
来源：http://xka.aizwys.cn

Ruby: Time.now
来源：http://dus.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fnr.dashuyun.cn

[J02] 格式化输出
来源：http://sdq.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://flb.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yhn.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ahf.tianlin.xyz

TS:   d.toISOString()
来源：http://jyl.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://npn.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zaj.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://flp.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ila.haohaochexian.top

[J03] 字符串解析为日期
来源：http://vfp.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ohh.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rek.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://jdl.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://kxp.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://gst.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mwq.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://jri.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://grr.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://dvk.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pvr.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rsf.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uet.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ulm.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ehz.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://odw.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hac.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zqz.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://sev.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://huo.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vyn.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://avr.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwp.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://rzq.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://evq.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://qyc.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://mzh.havefunace.top

[J06] 计算两时间之差
来源：http://vwy.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://vpj.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://bzc.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gib.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ezl.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wcu.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://kbn.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://dpd.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://jvx.xuanzx.com

[J07] 比较两个日期
来源：http://tml.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://ykv.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bgr.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ene.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://kfo.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hox.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://doe.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://pnu.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://uyc.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://ccx.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pyj.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wut.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gfz.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pkz.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hde.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wiv.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yfy.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wrz.meibo888.top

[J09] 时区处理
来源：http://dgj.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vpy.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uax.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtg.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xht.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://owc.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gjz.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zmp.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qcg.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://igt.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://hzn.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tsc.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zuq.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jwm.sjlbkw.cn


<!-- 参考信息 -->