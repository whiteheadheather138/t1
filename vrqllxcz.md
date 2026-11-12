代发 wailian999

Java: interface Shape { double area(); }
来源：http://bje.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://bhq.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cyn.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://zso.yuxming.cn

[G10] 访问控制
来源：http://xfh.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://unx.chenzaomai.com

PHP:  public / protected / private
来源：http://udr.havefunace.top

JS:   #private 字段；其余公开
来源：http://qfy.yuxming.cn

TS:   public / protected / private
来源：http://udx.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://rjb.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vej.dashuyun.cn

Ruby: public / protected / private
来源：http://gez.iojbl.cn

C#:   public / protected / private / internal
来源：http://emt.ybcxt.top

[G11] getter / setter
来源：http://upx.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://yxn.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://caw.birdmap.top

JS:   get name() { return this._name; }
来源：http://rey.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://oqo.yj202588.top

Java: public String getName() { return name; }
来源：http://yph.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rtl.meibo888.top

Ruby: attr_accessor :name
来源：http://tdg.uphjek.com

C#:   public string Name { get; set; }
来源：http://mfu.guowangkeji.top

[G12] 对象转字符串
来源：http://qpq.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://xkh.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ifj.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://dcg.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://poo.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://vmc.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vmc.smart0.xyz

Ruby: def to_s; @name; end
来源：http://jtq.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://zdd.zdbjq.cn

[G13] 判断对象类型
来源：http://hea.sweek.top

Py:   isinstance(u, User)
来源：http://jhg.shuidangran.top

PHP:  $u instanceof User
来源：http://rqj.hysaishi.cn

JS:   u instanceof User
来源：http://mus.c1oappe.top

TS:   u instanceof User
来源：http://bwr.gogol.net.cn

Java: u instanceof User
来源：http://cdh.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pyy.52xcode.cn

Ruby: u.is_a?(User)
来源：http://ptu.ydjk.org.cn

C#:   u is User
来源：http://eud.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://jci.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fqu.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://rpw.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://nyw.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://pus.andypj.xyz

Java: record User(String name, int age) {}
来源：http://rrm.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://yso.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nzz.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://npx.gotoacloud.top

[G15] 枚举
来源：http://ljr.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bho.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wui.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pix.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ppp.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://iww.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nmv.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://lwa.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hkb.uphjek.com

[G16] 对象转数组 / 字典
来源：http://cox.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tjy.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://kps.tian-w.cn

JS:   Object.entries(obj)
来源：http://wsz.nanxinkj.top

TS:   Object.entries(obj)
来源：http://qlh.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jfh.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://udg.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://cpd.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://gfe.316326.xyz

================================================================================
来源：http://jzv.gotoacloud.top

H. 异常与错误处理
来源：http://him.kuanghao11.cn

================================================================================
来源：http://xap.gotoacloud.top

[H01] try / catch 基础
来源：http://llc.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ajq.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mcg.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ssx.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lqr.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cfc.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jlj.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://guu.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kzi.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://wjg.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://pod.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sly.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://opq.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ala.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://cln.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://eby.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://evy.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dcp.daria6918.cn

[H03] 主动抛出异常
来源：http://jdv.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://mzc.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tcs.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://did.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://jvn.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xfq.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jmy.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aop.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fjj.52xcode.cn

[H04] 自定义异常类型
来源：http://arj.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://hmw.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xpl.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://qqo.jianghu66.top

TS:   class MyError extends Error {}
来源：http://gca.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://clx.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jdm.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://vkf.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://cqq.yj20258888.top

[H05] 捕获特定类型
来源：http://zqp.mhx1999.top

Py:   except ValueError as e:
来源：http://mrm.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xap.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://ppj.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://gaq.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://vvx.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://djj.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://nga.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://faw.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://vuf.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://xxp.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://tov.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://pgb.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://edh.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zkc.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ode.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://efd.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://fyp.fzhhl.top

[H07] 断言
来源：http://veh.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://ruo.tian-w.cn

PHP:  assert($x > 0);
来源：http://lbv.bjfxy.top

JS:   console.assert(x > 0);
来源：http://zaf.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://ymb.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://jeq.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fwv.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://zhg.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://zug.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://xal.daria6918.cn

Py:   str(e);  traceback.format_exc()
来源：http://hyq.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tyj.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://egk.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://axf.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wbp.xylfe.cn

Go:   err.Error()
来源：http://ixx.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://uly.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://rhe.hfpthk.cn

[H09] 带错误码的异常
来源：http://wgf.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://prz.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cza.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dkm.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjn.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rni.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zvn.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://dwc.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rdp.jlsjyb.cn

[H10] 资源自动释放
来源：http://ppq.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sun.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://frj.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hea.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://job.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rxf.yuanzhike.top

Go:   defer f.Close()
来源：http://jgv.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tah.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vvc.nanxuanxn.top

================================================================================
来源：http://vvu.316326.xyz

I. 正则表达式
来源：http://haw.xylfe.cn

================================================================================
来源：http://cqt.pycfn.com

[I01] 判断是否匹配
来源：http://qcf.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wqx.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://cgg.ivvv.top

JS:   /\d+/.test(s)
来源：http://xtg.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://alv.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oof.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://okt.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://zge.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vgu.nanxuanxn.top

[I02] 提取所有匹配
来源：http://isv.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://zeb.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dcn.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iov.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://bgv.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://png.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mic.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://otd.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zau.smart0.xyz

[I03] 提取捕获分组
来源：http://zxg.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jyj.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tem.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uqp.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://acz.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nsl.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mgx.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dxy.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://txk.cashguo.top

[I04] 正则替换
来源：http://qkj.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dzm.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tuc.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://rgl.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://qwa.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jjs.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vvx.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ooz.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pcd.tian-w.cn

[I05] 按正则拆分
来源：http://gpq.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mnw.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nop.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://xei.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://rdg.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://nol.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ubz.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://ecm.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uue.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mfr.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pga.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gvh.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdm.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dvj.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lqb.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://moe.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yhg.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rsu.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://ppy.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fjd.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ygl.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://akk.hammf.cn

TS:   /error/gim
来源：http://qko.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dwf.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ham.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://zfg.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ntx.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://tlo.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ebp.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yxd.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwp.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jrp.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tne.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oto.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://avr.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nna.shanyushiyangkeji.top

================================================================================
来源：http://iym.hesvh.cn

J. 日期与时间
来源：http://nxc.hcnkem.com

================================================================================
来源：http://iwv.nanxinkj.top

[J01] 获取当前时间
来源：http://fxu.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://pis.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vpv.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://lob.yueranfly.top

TS:   new Date();  Date.now()
来源：http://xtb.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bhq.shanyushiyangkeji.top

Go:   time.Now()
来源：http://dmy.daxiang520.top

Ruby: Time.now
来源：http://uvf.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://upn.hammf.cn

[J02] 格式化输出
来源：http://jvs.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tzx.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bfp.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://usq.sufxvd.cn

TS:   d.toISOString()
来源：http://jay.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fph.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uuo.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ppy.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jcx.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://bly.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cqf.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hgq.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://xkl.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://eyu.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://jfv.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://afg.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://noq.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wgv.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://cfk.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ses.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sfq.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqg.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://znw.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wbr.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bfq.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://twx.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nim.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://bas.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://kvs.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://btk.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tsn.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfq.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://ysn.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tyl.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://leo.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://tpp.hfpthk.cn

[J06] 计算两时间之差
来源：http://wve.tarul.cn

Py:   (end - start).total_seconds()
来源：http://gui.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://pwn.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ary.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ohv.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cax.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://jue.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://cfd.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://low.zhijiandao.cn

[J07] 比较两个日期
来源：http://dib.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://brc.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wms.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://ldp.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://kqg.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qel.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lqv.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://erp.svipenyu.cn


<!-- 参考信息 -->