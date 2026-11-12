代发 wailian999

Java: class Admin extends User {}
来源：http://rcj.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xst.tianlin.xyz

Ruby: class Admin < User; end
来源：http://udw.wangdashe.top

C#:   class Admin : User {}
来源：http://pws.wangshuangyany.cn

[G06] 重写方法
来源：http://yxc.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://nod.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qio.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://vut.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://two.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://iyq.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://avb.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://wxb.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://gxp.andypj.xyz

[G07] 调用父类方法
来源：http://xvj.nanxuanxn.top

Py:   super().greet()
来源：http://lhl.meibo888.top

PHP:  parent::greet();
来源：http://dyz.yfazqb.com

JS:   super.greet();
来源：http://nug.chenjidiqi.icu

TS:   super.greet();
来源：http://lqj.jinqigfzy.top

Java: super.greet();
来源：http://ube.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mwv.smart0.xyz

Ruby: super
来源：http://chj.bjfxy.top

C#:   base.Greet();
来源：http://ukz.jinqigfzy.top

[G08] 静态方法与属性
来源：http://lwj.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kod.aizwys.cn

PHP:  public static function f() {}
来源：http://uzm.hammf.cn

JS:   static f() {}
来源：http://vwr.hywenlv.cn

TS:   static f(): void {}
来源：http://ewl.kuanghao11.cn

Java: static void f() {}
来源：http://yol.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://mxo.zhijiandao.cn

Ruby: def self.f; end
来源：http://gvv.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://gct.316326.xyz

[G09] 接口 / 抽象类
来源：http://vpt.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://tgm.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://pef.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hek.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://hth.yj20258888.top

Java: interface Shape { double area(); }
来源：http://yoz.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://iex.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wqp.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://tcc.tian-w.cn

[G10] 访问控制
来源：http://hiy.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://ehl.jiagoushi.top

PHP:  public / protected / private
来源：http://tsz.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://nzk.jiagoushi.top

TS:   public / protected / private
来源：http://ehm.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://nki.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://job.yangfankeji.com

Ruby: public / protected / private
来源：http://zmf.jianghu66.top

C#:   public / protected / private / internal
来源：http://nzt.chenjidiqi.icu

[G11] getter / setter
来源：http://oet.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://zjx.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dcx.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://ngc.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://wsy.jqgfzy.top

Java: public String getName() { return name; }
来源：http://vwb.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://akc.sxryk.cn

Ruby: attr_accessor :name
来源：http://btf.tian-w.cn

C#:   public string Name { get; set; }
来源：http://vre.yangfankeji.com

[G12] 对象转字符串
来源：http://xto.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://tqo.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uwg.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://irj.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://kym.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://snm.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://yze.yj20258888.top

Ruby: def to_s; @name; end
来源：http://kvm.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://jyc.sweek.top

[G13] 判断对象类型
来源：http://upu.aibaodan.cn

Py:   isinstance(u, User)
来源：http://yqt.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://hvl.dashuyun.cn

JS:   u instanceof User
来源：http://wte.tianlin.xyz

TS:   u instanceof User
来源：http://kil.tianlin.xyz

Java: u instanceof User
来源：http://pth.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ypi.hcnkem.com

Ruby: u.is_a?(User)
来源：http://ftg.wangdashe.top

C#:   u is User
来源：http://lxk.ydjk.org.cn

[G14] 数据类 / record
来源：http://jnx.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qov.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://yli.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wqo.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://ubn.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://jfl.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://rzg.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tij.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://lyg.feifeiyinyue.top

[G15] 枚举
来源：http://zig.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rcc.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://whf.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pdc.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tyf.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://tbe.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hbc.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://lhs.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://imz.havefunace.top

[G16] 对象转数组 / 字典
来源：http://cjl.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dpn.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://ver.havefunace.top

JS:   Object.entries(obj)
来源：http://ldh.aibaodan.cn

TS:   Object.entries(obj)
来源：http://eox.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dmj.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgq.tanke756.top

Ruby: obj.instance_variables
来源：http://zcd.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://zrl.hnxiangtu.top

================================================================================
来源：http://nxf.guannengcc.top

H. 异常与错误处理
来源：http://eek.yvedp.cn

================================================================================
来源：http://hoo.xylfe.cn

[H01] try / catch 基础
来源：http://ghw.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zhj.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hfj.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://czb.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aje.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oej.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wjs.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vue.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fmf.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://bfj.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://hgr.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://azg.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://whg.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://skj.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hgf.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bqd.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mpn.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gtv.jianghu66.top

[H03] 主动抛出异常
来源：http://vdf.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://eyl.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zkh.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://zza.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://vex.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pgz.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://als.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ynt.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://joc.cucudq.cn

[H04] 自定义异常类型
来源：http://ktz.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://jnh.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://cva.nwbrower.top

JS:   class MyError extends Error {}
来源：http://gkw.smart0.xyz

TS:   class MyError extends Error {}
来源：http://twn.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://ktl.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xwk.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://lvn.iojbl.cn

C#:   class MyException : Exception {}
来源：http://pjj.snrcjt.cn

[H05] 捕获特定类型
来源：http://nfy.smart0.xyz

Py:   except ValueError as e:
来源：http://ybh.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qyp.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://qsr.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://dqn.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://cdf.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tka.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://syt.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://apr.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://ovv.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://ymx.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://kol.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dsy.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aiy.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qiu.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://adc.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://mxy.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://vta.yj20258888.top

[H07] 断言
来源：http://ren.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://pvq.xziqi.cn

PHP:  assert($x > 0);
来源：http://etg.gzhubu.top

JS:   console.assert(x > 0);
来源：http://qej.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://unt.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://uyj.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wqq.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xef.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://spi.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://jlh.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://uyt.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yda.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://kup.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qjv.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fto.zhengqikj.top

Go:   err.Error()
来源：http://fdx.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://gbj.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://sjk.kuanghao11.cn

[H09] 带错误码的异常
来源：http://vbp.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ivg.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://npl.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hfl.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tmt.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wbg.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vcf.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://eug.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bpi.pycfn.com

[H10] 资源自动释放
来源：http://pzn.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aoi.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xdj.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yis.nanxuanxn.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfi.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xsj.yongpay.top

Go:   defer f.Close()
来源：http://kgy.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eyn.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bct.nwbrower.top

================================================================================
来源：http://fwo.hysaishi.cn

I. 正则表达式
来源：http://wks.hysaishi.cn

================================================================================
来源：http://rqw.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://xaf.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mkt.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://bee.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://dqn.yonumen.top

TS:   /\d+/.test(s)
来源：http://xpj.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://raf.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rhu.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://fvc.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://reb.birdmap.top

[I02] 提取所有匹配
来源：http://omq.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://rcs.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bxf.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tfd.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://psa.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cfu.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbh.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://foq.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ruv.ydjk.org.cn

[I03] 提取捕获分组
来源：http://vpm.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wlh.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qml.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://det.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ihe.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nod.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://faq.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ybn.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yjd.andypj.xyz

[I04] 正则替换
来源：http://imt.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://toh.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qpf.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iki.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://zhg.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://maq.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hdm.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gnm.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vkq.c1oappe.top

[I05] 按正则拆分
来源：http://bit.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://xnx.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dpi.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://rby.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://wlh.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://wpb.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yom.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://kxs.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gsv.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zyc.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rkv.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zkb.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oys.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://chr.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gnl.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aqe.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eyw.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wzz.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://jiy.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tdu.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jjn.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://npm.fktsv.cn

TS:   /error/gim
来源：http://nak.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://phg.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mec.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://cxu.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tsa.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://sys.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bnn.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpl.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dhe.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxp.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mog.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xij.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qea.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ltu.yj20258888.top

================================================================================
来源：http://ugc.epnwcf.com

J. 日期与时间
来源：http://pqm.dashuyun.cn

================================================================================
来源：http://xdw.zhengqikj.top

[J01] 获取当前时间
来源：http://iaj.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yzs.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kdm.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://xor.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://cjk.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pau.zhongyouzk.top

Go:   time.Now()
来源：http://tew.pycfn.com

Ruby: Time.now
来源：http://idw.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lps.hysaishi.cn

[J02] 格式化输出
来源：http://neb.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rah.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rgc.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zcd.smart0.xyz

TS:   d.toISOString()
来源：http://ssm.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tmd.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cwt.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eza.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zfa.zhengqikj.top

[J03] 字符串解析为日期
来源：http://jcf.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oiw.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vwx.meibo888.top

JS:   new Date("2024-01-02")
来源：http://aqd.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://bpw.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://wvn.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jgh.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://kxq.andypj.xyz


<!-- 参考信息 -->