代发 wailian999

JS:   get name() { return this._name; }
来源：http://nwc.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://uzn.gzhubu.top

Java: public String getName() { return name; }
来源：http://cet.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ygk.hysaishi.cn

Ruby: attr_accessor :name
来源：http://ylo.c1oappe.top

C#:   public string Name { get; set; }
来源：http://uim.xuanzx.com

[G12] 对象转字符串
来源：http://hvx.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://unk.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://znf.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://jio.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://nkw.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://lue.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://avh.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://jhp.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://nwf.cheryme.top

[G13] 判断对象类型
来源：http://btp.yuxming.cn

Py:   isinstance(u, User)
来源：http://ore.yj202588.top

PHP:  $u instanceof User
来源：http://dtu.yj20258.top

JS:   u instanceof User
来源：http://uom.xuanzx.com

TS:   u instanceof User
来源：http://lyg.yuanzhike.top

Java: u instanceof User
来源：http://lhp.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vye.birdmap.top

Ruby: u.is_a?(User)
来源：http://uvc.bjfxy.top

C#:   u is User
来源：http://ans.jqgfzy.top

[G14] 数据类 / record
来源：http://fex.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oqw.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://qdv.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://vek.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://ick.fzhhl.top

Java: record User(String name, int age) {}
来源：http://tke.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://cba.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iow.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://puz.dianchejie.cn

[G15] 枚举
来源：http://pni.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rbp.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://eob.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yol.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://skn.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://qwt.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jhf.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://lpw.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fgs.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://niq.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wmx.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://btc.shuidangran.top

JS:   Object.entries(obj)
来源：http://sqz.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://ear.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vll.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://esz.yvedp.cn

Ruby: obj.instance_variables
来源：http://tma.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://kic.guannengcc.top

================================================================================
来源：http://vmp.xuetiantiany.cn

H. 异常与错误处理
来源：http://jed.shangyingyoupin.top

================================================================================
来源：http://oms.cucudq.cn

[H01] try / catch 基础
来源：http://gox.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cmp.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjt.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ylk.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sdp.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pho.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kvw.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fwj.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zla.sysykeji.top

[H02] finally / ensure 收尾
来源：http://nha.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://pww.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vva.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kuv.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vkd.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rqv.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://odh.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vec.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ixj.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://qpm.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://dsx.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vxx.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://rcp.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://hxf.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ohv.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://inu.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://cdp.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://qpu.yongpay.top

[H04] 自定义异常类型
来源：http://zhg.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://eti.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://baf.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://hhk.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://ekh.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://gtx.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hss.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://kdi.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://djt.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://lva.0kj1m.cn

Py:   except ValueError as e:
来源：http://ehj.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zdl.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://xtk.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://nat.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://pwk.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qja.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://wjb.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://asp.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://ggb.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://ixu.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://biq.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://imt.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://wxe.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ypi.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ljh.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://sdj.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://vtm.c1oappe.top

[H07] 断言
来源：http://kbc.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://mjz.cucudq.cn

PHP:  assert($x > 0);
来源：http://cdr.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://xce.fehbvm.com

TS:   console.assert(x > 0);
来源：http://itj.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://wrn.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ltg.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://osd.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://hfp.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://ovo.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://plf.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vkt.sysykeji.top

JS:   e.message;  e.stack
来源：http://rca.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vwp.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vqk.jqgfzy.top

Go:   err.Error()
来源：http://mru.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://apz.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://ede.ydjk.org.cn

[H09] 带错误码的异常
来源：http://xeu.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://igm.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://mtv.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zts.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dka.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sly.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yic.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://erc.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kdo.haohaochexian.top

[H10] 资源自动释放
来源：http://rre.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tcc.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gtm.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tnc.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://igc.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oio.52xcode.cn

Go:   defer f.Close()
来源：http://xxu.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xud.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yzg.ehwqpu.com

================================================================================
来源：http://nmd.cdnleiting.top

I. 正则表达式
来源：http://ktp.gaohongyu789.top

================================================================================
来源：http://xux.wangdashe.top

[I01] 判断是否匹配
来源：http://akp.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lwc.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vuq.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://cuj.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://xdk.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wym.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kuv.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://lnr.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lyx.gzhubu.top

[I02] 提取所有匹配
来源：http://dvm.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://yxl.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gpy.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://org.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://fws.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nvz.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tvx.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://gxq.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rrl.tarul.cn

[I03] 提取捕获分组
来源：http://llk.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mnl.chenzaomai.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lqf.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pqr.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fpq.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sfa.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mhu.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pqh.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gfn.smart0.xyz

[I04] 正则替换
来源：http://pjf.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://gtz.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vvv.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://pvp.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nha.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://esk.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oqy.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ifr.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rrh.epnwcf.com

[I05] 按正则拆分
来源：http://kvt.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ryg.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uni.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://pau.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://vnu.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://tsc.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sbh.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://two.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gej.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cmh.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zyp.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://abk.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qox.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lhq.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sgs.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lri.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aii.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxu.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://cef.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jvg.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://neh.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ejg.zhaomingkeji.xyz

TS:   /error/gim
来源：http://pqd.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vld.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://krs.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://gtu.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gux.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://uyn.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rwg.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://exu.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tqe.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lvo.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ggb.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wss.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ugy.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fvf.jlsjyb.cn

================================================================================
来源：http://yxd.yueranfly.top

J. 日期与时间
来源：http://cmz.yvedp.cn

================================================================================
来源：http://lhv.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://ijw.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://svy.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fer.sweek.top

JS:   new Date();  Date.now()
来源：http://ylj.yongpay.top

TS:   new Date();  Date.now()
来源：http://ywo.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vcn.hesvh.cn

Go:   time.Now()
来源：http://gjk.cqqwz.cn

Ruby: Time.now
来源：http://ynw.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gmt.ydjk.org.cn

[J02] 格式化输出
来源：http://whj.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcx.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tzv.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mzl.zhiwuduotai.top

TS:   d.toISOString()
来源：http://wqr.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://akw.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgd.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nme.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bbq.redwolf501.top

[J03] 字符串解析为日期
来源：http://hem.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bpq.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://adm.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://yts.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://onm.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://kba.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ghr.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://oib.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lrf.fzhhl.top

[J04] 时间戳与日期互转
来源：http://uiy.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tep.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hky.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sfs.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nnc.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gpv.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ulm.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xoo.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wwm.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://ofa.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://wyd.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zlt.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xrg.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohs.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://cod.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jpa.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://wkc.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fxk.dianchejie.cn

[J06] 计算两时间之差
来源：http://qjh.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://mgi.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://aqn.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ejb.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ohk.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://ysz.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://hzx.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://jep.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://uee.jlsjyb.cn

[J07] 比较两个日期
来源：http://szs.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://bxx.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eck.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uek.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://aza.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rta.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vbd.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://lsg.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://oqp.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://qyk.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ivx.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kvx.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emv.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://osr.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vjt.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dwc.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyz.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eil.fzhhl.top

[J09] 时区处理
来源：http://usm.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cyv.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xmi.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okt.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://glc.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gwx.hammf.cn


<!-- 参考信息 -->