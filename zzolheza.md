代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqc.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://syd.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://uyp.dianchejie.cn

[G05] 继承
来源：http://deo.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://exu.hammf.cn

PHP:  class Admin extends User {}
来源：http://xva.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://vbx.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://bez.vqdsnc.cn

Java: class Admin extends User {}
来源：http://snu.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jqe.wangdashe.top

Ruby: class Admin < User; end
来源：http://zfa.xziqi.cn

C#:   class Admin : User {}
来源：http://dfw.feifeiyinyue.top

[G06] 重写方法
来源：http://bgp.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://jum.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lpk.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://qyp.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://oei.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://zxb.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uds.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://dnv.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://uli.nanxinkj.top

[G07] 调用父类方法
来源：http://kbs.jlsjyb.cn

Py:   super().greet()
来源：http://nrq.yvedp.cn

PHP:  parent::greet();
来源：http://axg.yj20258.top

JS:   super.greet();
来源：http://qwx.daxiang520.top

TS:   super.greet();
来源：http://vdp.cucudq.cn

Java: super.greet();
来源：http://iby.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hdh.sufxvd.cn

Ruby: super
来源：http://hrt.yj202588.top

C#:   base.Greet();
来源：http://qks.fktsv.cn

[G08] 静态方法与属性
来源：http://eyk.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bsr.hywenlv.cn

PHP:  public static function f() {}
来源：http://sjq.jiagoushi.top

JS:   static f() {}
来源：http://ekl.c1oappe.top

TS:   static f(): void {}
来源：http://alh.andypj.xyz

Java: static void f() {}
来源：http://pnq.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xxd.gzhubu.top

Ruby: def self.f; end
来源：http://kxh.gotoacloud.top

C#:   public static void F() {}
来源：http://ypn.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://gqf.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://tid.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://izs.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://dfk.bjfxy.top

TS:   interface Shape { area(): number; }
来源：http://chr.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://kqm.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://aag.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qpl.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://qqq.daria6918.cn

[G10] 访问控制
来源：http://xmr.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://wys.chenzaomai.com

PHP:  public / protected / private
来源：http://qik.ivvv.top

JS:   #private 字段；其余公开
来源：http://lig.yvedp.cn

TS:   public / protected / private
来源：http://iae.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://eaj.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rpj.52xcode.cn

Ruby: public / protected / private
来源：http://isb.52xcode.cn

C#:   public / protected / private / internal
来源：http://aox.gzhubu.top

[G11] getter / setter
来源：http://kqf.yueranfly.top

Py:   @property 与 @x.setter
来源：http://ikh.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kfg.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://muc.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://snu.xinyue.icu

Java: public String getName() { return name; }
来源：http://jwl.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hqh.zycfv.cn

Ruby: attr_accessor :name
来源：http://asf.daxiang520.top

C#:   public string Name { get; set; }
来源：http://vhz.wangdashe.top

[G12] 对象转字符串
来源：http://kwn.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://ide.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nru.zycfv.cn

JS:   toString() { return this.name; }
来源：http://juz.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://fwh.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://xhw.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://jxu.xinyue.icu

Ruby: def to_s; @name; end
来源：http://nsg.yj20258.top

C#:   public override string ToString() => Name;
来源：http://gay.jyoumei.cn

[G13] 判断对象类型
来源：http://xdo.hesvh.cn

Py:   isinstance(u, User)
来源：http://iob.chenlongwang.top

PHP:  $u instanceof User
来源：http://zna.snrcjt.cn

JS:   u instanceof User
来源：http://sif.pengpengdd.cyou

TS:   u instanceof User
来源：http://ysn.yuxming.cn

Java: u instanceof User
来源：http://zkb.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mce.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://cab.gogol.net.cn

C#:   u is User
来源：http://zpa.zhoulong.xyz

[G14] 数据类 / record
来源：http://bby.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ehm.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://wtd.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fkp.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://irk.bbcook.cn

Java: record User(String name, int age) {}
来源：http://too.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://xil.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qmr.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://adc.smart0.xyz

[G15] 枚举
来源：http://pqu.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xdw.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://teb.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jgs.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vvu.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://def.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wxd.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://qlq.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bas.ivvv.top

[G16] 对象转数组 / 字典
来源：http://ruy.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://czx.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://nan.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://vsh.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://hnd.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://spa.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nla.yuxming.cn

Ruby: obj.instance_variables
来源：http://tus.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://gyd.guowangkeji.top

================================================================================
来源：http://yqb.hywenlv.cn

H. 异常与错误处理
来源：http://wal.iojbl.cn

================================================================================
来源：http://ihr.meibo888.top

[H01] try / catch 基础
来源：http://unx.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pha.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rgn.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wvb.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fgc.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qnl.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://btv.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lot.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pld.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://aze.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jji.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ohr.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dox.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oea.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xcn.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://alf.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://yts.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ndv.jlsjyb.cn

[H03] 主动抛出异常
来源：http://gpn.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://ken.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ops.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://cnk.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://nls.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vmb.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jqf.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://noe.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qvg.ydzc1.top

[H04] 自定义异常类型
来源：http://udt.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://rnd.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://chf.uphjek.com

JS:   class MyError extends Error {}
来源：http://tqj.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://ebe.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://jst.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ysl.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://kgv.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://xex.xuanzx.com

[H05] 捕获特定类型
来源：http://syl.yonumen.top

Py:   except ValueError as e:
来源：http://ncp.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gyn.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://kbq.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://anc.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://hio.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://czr.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://tug.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tjq.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://fgh.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://ogo.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://imk.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://pny.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://muk.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vzp.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ceh.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://ddi.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://zeo.nanxinkj.top

[H07] 断言
来源：http://vos.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://rdv.ctjpmb.com

PHP:  assert($x > 0);
来源：http://ets.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://jqi.yj20258888.top

TS:   console.assert(x > 0);
来源：http://qgs.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://unt.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vmm.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pru.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://ucl.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://olw.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://ajj.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ifq.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://vhs.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgt.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jnd.epnwcf.com

Go:   err.Error()
来源：http://hwc.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://ivm.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://hmc.fengsongda.top

[H09] 带错误码的异常
来源：http://uyu.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ysm.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ofg.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://unh.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://odq.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ily.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zer.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://kop.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tjr.smart0.xyz

[H10] 资源自动释放
来源：http://dmp.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dsw.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kuv.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mzx.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ojv.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://spr.yuanzhike.top

Go:   defer f.Close()
来源：http://pzg.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rsi.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uzv.0kj1m.cn

================================================================================
来源：http://vkc.chenjidiqi.icu

I. 正则表达式
来源：http://fmk.wangshuangyany.cn

================================================================================
来源：http://blr.yuanzhike.top

[I01] 判断是否匹配
来源：http://bpb.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yqv.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://ewi.xylfe.cn

JS:   /\d+/.test(s)
来源：http://mfe.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://gdz.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://grt.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gug.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://llb.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mqk.9152youxi.cn

[I02] 提取所有匹配
来源：http://wbs.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://pqc.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jiq.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://btk.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://cbh.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jup.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://krz.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://fpa.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ylb.smart0.xyz

[I03] 提取捕获分组
来源：http://lqs.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://njg.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mza.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ofi.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lnc.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cit.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uta.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ndg.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bem.zycfv.cn

[I04] 正则替换
来源：http://zxw.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gyr.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fqy.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://tng.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pum.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://tcq.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://zzv.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hbt.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://juz.shzxlz.cn

[I05] 按正则拆分
来源：http://cya.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vvm.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fyj.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://hbv.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://hiu.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://tyk.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mfv.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mek.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://evk.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://brr.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vln.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pmt.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nle.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkk.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uvx.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://omg.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://afh.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ahd.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://tvg.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lsq.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hpm.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hek.sweek.top

TS:   /error/gim
来源：http://bxe.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ptk.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xvm.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://dcg.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://prz.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://uhd.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vzm.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ihd.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nsc.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hos.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ium.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iqm.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwp.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://huh.xziqi.cn

================================================================================
来源：http://vbp.xuanzx.com

J. 日期与时间
来源：http://bne.hfpthk.cn

================================================================================
来源：http://upq.cucudq.cn

[J01] 获取当前时间
来源：http://skh.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://sdc.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://coi.sweek.top

JS:   new Date();  Date.now()
来源：http://rsq.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://fla.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kcs.aizwys.cn

Go:   time.Now()
来源：http://wug.sufxvd.cn

Ruby: Time.now
来源：http://jgq.yvedp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lrs.havefunace.top

[J02] 格式化输出
来源：http://gvm.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uzs.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wog.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oid.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://qcp.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cdw.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ekm.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjs.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qde.jlsjyb.cn


<!-- 参考信息 -->