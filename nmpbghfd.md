代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://fqj.hnqzz.top

[G07] 调用父类方法
来源：http://szq.nanxuanxn.top

Py:   super().greet()
来源：http://bjw.dashuyun.cn

PHP:  parent::greet();
来源：http://cbl.jlsjyb.cn

JS:   super.greet();
来源：http://lso.cucudq.cn

TS:   super.greet();
来源：http://lhv.hywenlv.cn

Java: super.greet();
来源：http://epw.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lbq.hnqzz.top

Ruby: super
来源：http://lil.shanyushiyangtech.top

C#:   base.Greet();
来源：http://jyo.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://jnq.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jdh.ppjwa.cn

PHP:  public static function f() {}
来源：http://upm.zhoulong.xyz

JS:   static f() {}
来源：http://kvj.kuanghao11.cn

TS:   static f(): void {}
来源：http://dxh.sjlbkw.cn

Java: static void f() {}
来源：http://njm.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://bhu.bjfxy.top

Ruby: def self.f; end
来源：http://jqp.zhiwuduotai.top

C#:   public static void F() {}
来源：http://hde.zycfv.cn

[G09] 接口 / 抽象类
来源：http://bdm.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ihl.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://wii.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bpa.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://yoo.tian-w.cn

Java: interface Shape { double area(); }
来源：http://yxn.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://rjw.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qrd.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://uxo.hnqzz.top

[G10] 访问控制
来源：http://htu.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://kfg.zdqjudy.top

PHP:  public / protected / private
来源：http://hgy.hnqzz.top

JS:   #private 字段；其余公开
来源：http://yuw.cheryme.top

TS:   public / protected / private
来源：http://lkv.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://jqe.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://snv.gzhubu.top

Ruby: public / protected / private
来源：http://gmk.vehdjk.com

C#:   public / protected / private / internal
来源：http://kbh.jyoumei.cn

[G11] getter / setter
来源：http://uzp.yfazqb.com

Py:   @property 与 @x.setter
来源：http://rfl.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://qkg.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://ksv.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://qgy.ybcxt.top

Java: public String getName() { return name; }
来源：http://dei.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://duz.fzhhl.top

Ruby: attr_accessor :name
来源：http://lnm.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://ezy.xuanzx.com

[G12] 对象转字符串
来源：http://hsu.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://jyr.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sbz.yj20258.top

JS:   toString() { return this.name; }
来源：http://hhd.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://olj.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://pym.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://blk.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://yfw.tarul.cn

C#:   public override string ToString() => Name;
来源：http://udh.jlsjyb.cn

[G13] 判断对象类型
来源：http://gjb.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://wor.jinqigufen.top

PHP:  $u instanceof User
来源：http://pkq.tarul.cn

JS:   u instanceof User
来源：http://ihm.hcnkem.com

TS:   u instanceof User
来源：http://hsa.smart0.xyz

Java: u instanceof User
来源：http://ros.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ybn.iojbl.cn

Ruby: u.is_a?(User)
来源：http://qqr.guannengcc.top

C#:   u is User
来源：http://arf.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://ptb.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iyf.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://lhs.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://hex.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://voq.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://ulp.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://aky.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jul.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://hku.jqgufenzy.top

[G15] 枚举
来源：http://wkw.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://laf.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mwo.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uta.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fpv.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://uqi.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ygv.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://dip.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fsq.yj202588.top

[G16] 对象转数组 / 字典
来源：http://ker.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zsc.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://dgf.hammf.cn

JS:   Object.entries(obj)
来源：http://qmm.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://bkr.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hhw.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lxi.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://vxi.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://fbv.ppjwa.cn

================================================================================
来源：http://htl.52xcode.cn

H. 异常与错误处理
来源：http://ekm.xinyue.icu

================================================================================
来源：http://mfa.epnwcf.com

[H01] try / catch 基础
来源：http://xup.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://igf.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://njm.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ycr.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lto.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qge.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vcz.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bjq.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jqd.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://ics.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://pei.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ddr.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fjd.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://frg.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://gtd.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tsu.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qoe.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://fuc.jinqigufen.top

[H03] 主动抛出异常
来源：http://ysz.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://tqm.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mnx.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://eid.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://kgc.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eaa.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://afi.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gyh.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pnp.iojbl.cn

[H04] 自定义异常类型
来源：http://afy.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://fti.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://nht.hcnkem.com

JS:   class MyError extends Error {}
来源：http://zvv.pycfn.com

TS:   class MyError extends Error {}
来源：http://alm.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://ijv.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xoa.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://hkm.fehbvm.com

C#:   class MyException : Exception {}
来源：http://bdr.hysaishi.cn

[H05] 捕获特定类型
来源：http://xda.ybcxt.top

Py:   except ValueError as e:
来源：http://dhr.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://owb.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://nuq.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://zma.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://ufv.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uul.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://tyv.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://buw.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://bjl.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://uhi.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qky.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fuv.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://xaj.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dlv.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yzb.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://prr.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://fqy.ydzc1.top

[H07] 断言
来源：http://ypt.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://ypo.chenzaomai.com

PHP:  assert($x > 0);
来源：http://bqx.cucudq.cn

JS:   console.assert(x > 0);
来源：http://inp.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://uey.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ryw.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://atd.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://kto.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://ong.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://rwp.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://jcm.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lis.bjfxy.top

JS:   e.message;  e.stack
来源：http://dth.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://euj.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bkj.yangfankeji.com

Go:   err.Error()
来源：http://ifp.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://rno.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://jdd.xuanzx.com

[H09] 带错误码的异常
来源：http://sta.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ytb.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://fdj.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hvf.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://axk.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://naa.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cjd.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://kou.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qic.kuanghao11.cn

[H10] 资源自动释放
来源：http://uni.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qte.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qiy.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lfg.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ykg.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qma.snrcjt.cn

Go:   defer f.Close()
来源：http://hfy.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dds.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ylq.jinqigfzy.top

================================================================================
来源：http://qyf.xingfuxueyuan.xyz

I. 正则表达式
来源：http://ykj.tanke756.top

================================================================================
来源：http://pzs.cucudq.cn

[I01] 判断是否匹配
来源：http://mvb.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jve.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ypd.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://qkn.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://kwg.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oam.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://chn.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://vba.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ode.jinqigfzy.top

[I02] 提取所有匹配
来源：http://ulk.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://meh.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xnz.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://efu.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://rpl.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fsr.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fmq.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://mog.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://npz.cheryme.top

[I03] 提取捕获分组
来源：http://uje.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tbr.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://frx.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oid.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzy.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ujr.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hia.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nnt.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rpt.fktsv.cn

[I04] 正则替换
来源：http://myh.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://htb.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jfb.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uuw.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://hvo.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://dmj.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://xjj.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ofa.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://spb.sxryk.cn

[I05] 按正则拆分
来源：http://uvp.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bwp.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dgn.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://stt.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://lcb.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://haj.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bpy.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://yqa.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xok.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fyy.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://srp.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kgp.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wtk.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kyn.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qdk.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fku.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ahv.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://boa.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://uhn.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vyh.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iot.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pqx.meibo888.top

TS:   /error/gim
来源：http://yyb.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rvb.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mco.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://umz.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ebg.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://ydf.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iwr.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsm.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qsv.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zxf.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gmc.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://miz.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://liq.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://axg.snrcjt.cn

================================================================================
来源：http://gjs.fzhhl.top

J. 日期与时间
来源：http://lmj.gotoacloud.top

================================================================================
来源：http://mzw.fktsv.cn

[J01] 获取当前时间
来源：http://azt.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fgp.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yeo.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://pjv.yfazqb.com

TS:   new Date();  Date.now()
来源：http://xcw.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zvb.jianghu66.top

Go:   time.Now()
来源：http://jxk.tarul.cn

Ruby: Time.now
来源：http://nuk.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xxo.yonumen.top

[J02] 格式化输出
来源：http://xml.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wra.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tto.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vyk.daria6918.cn

TS:   d.toISOString()
来源：http://itf.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jmu.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://smy.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgf.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kzt.yonumen.top

[J03] 字符串解析为日期
来源：http://whh.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://myq.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xbc.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://dxi.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://yyt.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://cll.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lru.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://wnq.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gum.yj20258.top

[J04] 时间戳与日期互转
来源：http://roo.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lud.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dff.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ren.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://evs.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iwk.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eip.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cmn.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kws.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://ivv.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://rte.fanxiaobao.xyz


<!-- 参考信息 -->