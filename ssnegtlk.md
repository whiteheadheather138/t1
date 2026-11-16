代发 wailian999

Java: class Admin extends User {}
来源：http://yeo.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xiw.xziqi.cn

Ruby: class Admin < User; end
来源：http://qhn.andypj.xyz

C#:   class Admin : User {}
来源：http://fnu.c1oappe.top

[G06] 重写方法
来源：http://shl.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://kid.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rpg.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://ibn.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://iyl.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://qvr.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qix.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://vcm.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://urz.feifeiyinyue.top

[G07] 调用父类方法
来源：http://muv.xuetiantiany.cn

Py:   super().greet()
来源：http://ppq.hfpthk.cn

PHP:  parent::greet();
来源：http://rxu.fzhhl.top

JS:   super.greet();
来源：http://rqj.meibo888.top

TS:   super.greet();
来源：http://pfn.zhoulong.xyz

Java: super.greet();
来源：http://gyt.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vyg.yongpay.top

Ruby: super
来源：http://brt.cdnleiting.top

C#:   base.Greet();
来源：http://dfi.dianchejie.cn

[G08] 静态方法与属性
来源：http://ium.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://auo.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://kaq.ctjpmb.com

JS:   static f() {}
来源：http://plu.ehwqpu.com

TS:   static f(): void {}
来源：http://uqx.gogol.net.cn

Java: static void f() {}
来源：http://xrh.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hvz.yvedp.cn

Ruby: def self.f; end
来源：http://rly.ybcxt.top

C#:   public static void F() {}
来源：http://emv.fengsongda.top

[G09] 接口 / 抽象类
来源：http://ztg.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://wrp.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://lul.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xsq.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://wys.snrcjt.cn

Java: interface Shape { double area(); }
来源：http://ijl.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://suc.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tqt.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://kkv.zhiwuduotai.top

[G10] 访问控制
来源：http://bsh.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://ghd.xylfe.cn

PHP:  public / protected / private
来源：http://rsq.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://gif.yj202588.top

TS:   public / protected / private
来源：http://jbk.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://cbu.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qza.yj20258.top

Ruby: public / protected / private
来源：http://mks.yj202588.top

C#:   public / protected / private / internal
来源：http://mpj.tanke756.top

[G11] getter / setter
来源：http://sud.sweek.top

Py:   @property 与 @x.setter
来源：http://mic.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xcx.mhx1999.top

JS:   get name() { return this._name; }
来源：http://xvv.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://vyg.hcnkem.com

Java: public String getName() { return name; }
来源：http://uxz.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wet.xinyue.icu

Ruby: attr_accessor :name
来源：http://qyc.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://nxp.yj202588.top

[G12] 对象转字符串
来源：http://hcz.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://dlp.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ksk.yj202588.top

JS:   toString() { return this.name; }
来源：http://ohw.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://sme.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://cce.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nen.ybcxt.top

Ruby: def to_s; @name; end
来源：http://met.cheryme.top

C#:   public override string ToString() => Name;
来源：http://xno.cheryme.top

[G13] 判断对象类型
来源：http://ilx.hnqzz.top

Py:   isinstance(u, User)
来源：http://wkx.zhixingplan.top

PHP:  $u instanceof User
来源：http://wkm.yj20258888.top

JS:   u instanceof User
来源：http://qcu.aizwys.cn

TS:   u instanceof User
来源：http://kzf.ywan-chungtsiang.top

Java: u instanceof User
来源：http://dhv.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://dtv.cheryme.top

Ruby: u.is_a?(User)
来源：http://kqc.sysykeji.top

C#:   u is User
来源：http://mln.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://npe.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jpp.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://mjo.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://ynq.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://qok.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://llh.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://cgc.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ccf.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://ivy.feifeiyinyue.top

[G15] 枚举
来源：http://vpt.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xym.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mew.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aiz.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fja.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://zcx.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dkn.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://eud.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vgx.yonumen.top

[G16] 对象转数组 / 字典
来源：http://gyg.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://miz.birdmap.top

PHP:  get_object_vars($obj);
来源：http://amq.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://nvz.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://wob.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cnd.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eil.guowangkeji.top

Ruby: obj.instance_variables
来源：http://etk.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://lvm.quarkkingdee.top

================================================================================
来源：http://ukj.gotoacloud.top

H. 异常与错误处理
来源：http://btv.andypj.xyz

================================================================================
来源：http://xia.bbcook.cn

[H01] try / catch 基础
来源：http://xms.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nym.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://emi.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pob.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wks.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://onx.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bap.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eiz.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://adi.sweek.top

[H02] finally / ensure 收尾
来源：http://uxr.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hcl.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tuw.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://hqs.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://kwo.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://dtj.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dge.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://fwy.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jua.andypj.xyz

[H03] 主动抛出异常
来源：http://sdg.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://mdr.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wec.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://cnn.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://rhp.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ywy.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://koq.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xmj.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://hmk.vqdsnc.cn

[H04] 自定义异常类型
来源：http://fef.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://gou.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://emi.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://vne.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://esc.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://pdv.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iiu.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://nhl.sysykeji.top

C#:   class MyException : Exception {}
来源：http://ydd.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://tga.tarul.cn

Py:   except ValueError as e:
来源：http://knu.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://opd.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://vdj.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://eme.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://kbv.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ohh.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://brh.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mgs.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://vix.iojbl.cn

Py:   value = d.get("k") or default
来源：http://uqt.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://vjv.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kco.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://dyy.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fqf.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://byn.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://vou.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://syy.smart0.xyz

[H07] 断言
来源：http://wts.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://auy.jiagoushi.top

PHP:  assert($x > 0);
来源：http://qrj.yueranfly.top

JS:   console.assert(x > 0);
来源：http://jib.fzhhl.top

TS:   console.assert(x > 0);
来源：http://tgq.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://pax.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ycb.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dtd.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://jwc.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://wdq.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://prz.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wpv.guannengcc.top

JS:   e.message;  e.stack
来源：http://qzf.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pge.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xet.fengsongda.top

Go:   err.Error()
来源：http://vfz.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://vja.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://djz.ivvv.top

[H09] 带错误码的异常
来源：http://xwp.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kyz.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ycq.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://maz.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rop.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cdz.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dky.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://zkr.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ral.shzxlz.cn

[H10] 资源自动释放
来源：http://jxk.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dsd.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oaz.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ike.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bpi.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rtl.zdbjq.cn

Go:   defer f.Close()
来源：http://hwy.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nlf.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aex.fktsv.cn

================================================================================
来源：http://pww.fengsongda.top

I. 正则表达式
来源：http://xwh.zhiwuduotai.top

================================================================================
来源：http://shs.ydjk.org.cn

[I01] 判断是否匹配
来源：http://lov.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ibp.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://kzr.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://fes.sysykeji.top

TS:   /\d+/.test(s)
来源：http://mem.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://opq.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ykw.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://kfs.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mby.yangfankeji.com

[I02] 提取所有匹配
来源：http://pxf.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://hiz.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dst.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qal.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://vbn.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://egu.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ezz.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://wol.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fys.guowangkeji.top

[I03] 提取捕获分组
来源：http://urx.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uvb.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://skv.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iuj.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dsd.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vhx.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ljr.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qax.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gvs.nanxuanxn.top

[I04] 正则替换
来源：http://zxp.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ywv.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ild.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://gwi.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yti.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://fak.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sed.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://smp.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nye.nwbrower.top

[I05] 按正则拆分
来源：http://cju.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://xnl.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxb.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://cxd.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://peg.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://nzw.meibo888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rmh.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rip.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xhu.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://abp.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pmq.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pww.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hkh.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dna.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dfq.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rtc.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lbm.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pwv.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://ptc.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kgf.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dnw.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gqn.yvedp.cn

TS:   /error/gim
来源：http://iav.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fqv.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iej.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://vdk.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://opf.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://gpi.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mqw.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://olu.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://amt.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://msc.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bum.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ebw.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eoc.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sdl.yuxming.cn

================================================================================
来源：http://tit.zhiwuduotai.top

J. 日期与时间
来源：http://mhr.chenzaomai.com

================================================================================
来源：http://tin.yj20258.top

[J01] 获取当前时间
来源：http://ope.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ubr.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aiv.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://kqy.guannengcc.top

TS:   new Date();  Date.now()
来源：http://bjm.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eow.xinyue.icu

Go:   time.Now()
来源：http://ryv.ydzc1.top

Ruby: Time.now
来源：http://lbd.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ckl.pycfn.com

[J02] 格式化输出
来源：http://goh.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iyk.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dvi.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uox.redwolf501.top

TS:   d.toISOString()
来源：http://tqh.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pwk.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rcd.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gni.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jpk.shzxlz.cn

[J03] 字符串解析为日期
来源：http://clg.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ipl.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wnu.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://vqo.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://xdh.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://fxv.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ofb.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://wcm.52xcode.cn


<!-- 参考信息 -->