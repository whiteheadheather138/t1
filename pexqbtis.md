代发 wailian999

PHP:  public static function f() {}
来源：http://rdj.yuxming.cn

JS:   static f() {}
来源：http://rnb.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://lwh.chenlongwang.top

Java: static void f() {}
来源：http://xog.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fuj.yongpay.top

Ruby: def self.f; end
来源：http://vdx.hongshengwenyu.top

C#:   public static void F() {}
来源：http://dsl.hesvh.cn

[G09] 接口 / 抽象类
来源：http://wab.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://lel.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://ref.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fee.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://qpf.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://zpz.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://zpw.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kgx.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://pxj.yanxiufei.cn

[G10] 访问控制
来源：http://zkb.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://lji.havefunace.top

PHP:  public / protected / private
来源：http://pjl.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://ysn.cqqwz.cn

TS:   public / protected / private
来源：http://yzn.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://lay.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fcm.hfpthk.cn

Ruby: public / protected / private
来源：http://hxy.aizwys.cn

C#:   public / protected / private / internal
来源：http://led.cqqwz.cn

[G11] getter / setter
来源：http://vnw.ivvv.top

Py:   @property 与 @x.setter
来源：http://moi.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://fkg.uphjek.com

JS:   get name() { return this._name; }
来源：http://box.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://jxv.nwbrower.top

Java: public String getName() { return name; }
来源：http://cfe.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://qkw.zhixingplan.top

Ruby: attr_accessor :name
来源：http://nzo.uphjek.com

C#:   public string Name { get; set; }
来源：http://yqp.bjfxy.top

[G12] 对象转字符串
来源：http://jsm.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://lau.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yiy.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://kqo.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://fiw.sweek.top

Java: @Override public String toString() { return name; }
来源：http://sso.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nkv.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://gew.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://oae.shangyingyoupin.top

[G13] 判断对象类型
来源：http://tkf.smart0.xyz

Py:   isinstance(u, User)
来源：http://hft.birdmap.top

PHP:  $u instanceof User
来源：http://klm.hnqzz.top

JS:   u instanceof User
来源：http://rik.0kj1m.cn

TS:   u instanceof User
来源：http://uhi.tanke756.top

Java: u instanceof User
来源：http://hvw.wangdashe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rbz.sysykeji.top

Ruby: u.is_a?(User)
来源：http://yhv.tianlin.xyz

C#:   u is User
来源：http://vtf.yj20258.top

[G14] 数据类 / record
来源：http://qza.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://seo.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cbw.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://zzi.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://xuo.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://kxf.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://huc.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dcw.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://ynr.uphjek.com

[G15] 枚举
来源：http://mlv.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://smt.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jti.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ydy.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rjj.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://icm.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://puk.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://kez.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rph.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://pll.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mac.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://brn.iojbl.cn

JS:   Object.entries(obj)
来源：http://ray.hfpthk.cn

TS:   Object.entries(obj)
来源：http://wso.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ttl.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gyp.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://uav.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://zrd.xuetiantiany.cn

================================================================================
来源：http://sde.chenjidiqi.icu

H. 异常与错误处理
来源：http://xsc.sjlbkw.cn

================================================================================
来源：http://zsx.yanxiufei.cn

[H01] try / catch 基础
来源：http://yqy.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zqu.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xgn.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kls.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppz.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lvl.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oeo.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gul.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xqa.tian-w.cn

[H02] finally / ensure 收尾
来源：http://aun.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://jui.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wbm.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mmf.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sut.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://kpd.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ouo.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qcs.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gyt.sxryk.cn

[H03] 主动抛出异常
来源：http://fib.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://jvt.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://usk.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://ivw.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://djh.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://xhi.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wos.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://svw.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://fys.zhijiandao.cn

[H04] 自定义异常类型
来源：http://oui.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://tds.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://lqc.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://flk.cheryme.top

TS:   class MyError extends Error {}
来源：http://gqi.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://jsq.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qqr.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://ynp.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://gsk.chenlongwang.top

[H05] 捕获特定类型
来源：http://ygu.cucudq.cn

Py:   except ValueError as e:
来源：http://kaq.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pef.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://ipj.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://nue.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://vis.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://prw.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://juu.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xgm.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://tzh.yfazqb.com

Py:   value = d.get("k") or default
来源：http://qlj.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://cbs.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lxb.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://mcq.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hct.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xbl.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://tgj.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://wrq.dashuyun.cn

[H07] 断言
来源：http://ifu.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://mvi.0kj1m.cn

PHP:  assert($x > 0);
来源：http://tqf.nwbrower.top

JS:   console.assert(x > 0);
来源：http://aza.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://tvo.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://jnb.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://csi.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://eeg.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://neb.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://gvs.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://xfd.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jpb.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://xwz.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zwy.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://djp.smart0.xyz

Go:   err.Error()
来源：http://dhj.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://bgu.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://hbz.nanxuanxn.top

[H09] 带错误码的异常
来源：http://atm.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqu.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://zbf.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zzm.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jgw.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oez.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkc.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://jxt.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wki.gaohongyu789.top

[H10] 资源自动释放
来源：http://ljw.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://frq.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vlc.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jfx.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vsv.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yyp.fehbvm.com

Go:   defer f.Close()
来源：http://csy.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kck.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vtd.shangyingyoupin.top

================================================================================
来源：http://hdr.smart0.xyz

I. 正则表达式
来源：http://wmt.gzhubu.top

================================================================================
来源：http://fhz.guowangkeji.top

[I01] 判断是否匹配
来源：http://eih.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ekv.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ovx.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://mwj.redwolf501.top

TS:   /\d+/.test(s)
来源：http://wvk.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://txh.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xtd.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://lxm.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fxn.gogol.net.cn

[I02] 提取所有匹配
来源：http://bwb.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://aeh.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vrk.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnt.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://sbi.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://leq.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dpg.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://tpc.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ibl.yuxming.cn

[I03] 提取捕获分组
来源：http://pos.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oni.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kyu.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ton.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cbw.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fxn.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bkw.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qxm.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kne.guannengcc.top

[I04] 正则替换
来源：http://wdx.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://urc.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aca.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ckn.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://ysp.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hca.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mda.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://fjo.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ocq.hysaishi.cn

[I05] 按正则拆分
来源：http://mdq.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ggb.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bwc.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://bdc.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://elt.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://zfo.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tyj.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://vrr.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tof.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gpo.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zxv.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vlg.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dre.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ytq.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://loy.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://isi.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jjj.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ltg.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://npa.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ydq.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xdb.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mgq.nanxuanxn.top

TS:   /error/gim
来源：http://tvm.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xme.zhaomingkeji.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sdl.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://bxe.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ngx.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://wvg.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yzt.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qsy.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogm.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://chj.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://rrn.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sih.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://icw.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cdt.meibo888.top

================================================================================
来源：http://stm.jqgfzy.top

J. 日期与时间
来源：http://pmv.cheryme.top

================================================================================
来源：http://uaz.sweek.top

[J01] 获取当前时间
来源：http://zib.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rbm.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fgl.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://fdd.guannengcc.top

TS:   new Date();  Date.now()
来源：http://buv.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://yws.shzxlz.cn

Go:   time.Now()
来源：http://mjh.jinqigufen.top

Ruby: Time.now
来源：http://cdg.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vqd.yj20258888.top

[J02] 格式化输出
来源：http://amh.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgd.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lne.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zvs.zycfv.cn

TS:   d.toISOString()
来源：http://gnz.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vqy.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mdt.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://csy.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pji.mhx1999.top

[J03] 字符串解析为日期
来源：http://hew.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tvc.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ssn.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://gwe.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://hrs.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://zcy.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vdv.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://ekd.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pbf.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://udl.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://geb.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://miy.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vjy.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bur.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yil.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hrh.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tro.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dhb.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://xwc.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://job.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iup.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xnv.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtl.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://qxv.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tem.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://hcp.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bbh.uphjek.com

[J06] 计算两时间之差
来源：http://elo.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://apr.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://ogy.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jch.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mub.ivvv.top


<!-- 参考信息 -->