代发 wailian999

JS:   this.name = "x";
来源：http://yfp.ivvv.top

TS:   name: string = "x";
来源：http://cih.yj20258.top

Java: private String name;
来源：http://vrl.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jtw.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://eet.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://lry.dianchejie.cn

[G04] 定义方法
来源：http://htn.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://prr.tian-w.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yot.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://euq.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://cfk.havefunace.top

Java: String greet() { return name; }
来源：http://fjz.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aoo.ybcxt.top

Ruby: def greet; @name; end
来源：http://hxq.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://klj.tanke756.top

[G05] 继承
来源：http://vxz.yj20258888.top

Py:   class Admin(User): pass
来源：http://ild.xinyue.icu

PHP:  class Admin extends User {}
来源：http://tie.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://mtw.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://efk.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://eiv.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://arz.fehbvm.com

Ruby: class Admin < User; end
来源：http://apv.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://lwe.nanxinkj.top

[G06] 重写方法
来源：http://zjx.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://uqp.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://htq.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://gtx.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://hpm.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ltr.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uca.tarul.cn

Ruby: def greet; "admin"; end
来源：http://qax.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://edn.zdbjq.cn

[G07] 调用父类方法
来源：http://ttj.jiagoushi.top

Py:   super().greet()
来源：http://usx.haohaochexian.top

PHP:  parent::greet();
来源：http://cze.wangshuangyany.cn

JS:   super.greet();
来源：http://qdz.gogol.net.cn

TS:   super.greet();
来源：http://pwi.ctjpmb.com

Java: super.greet();
来源：http://gdd.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cyv.zycfv.cn

Ruby: super
来源：http://sgm.meibo888.top

C#:   base.Greet();
来源：http://obl.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://qaa.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mbz.kuanghao11.cn

PHP:  public static function f() {}
来源：http://kll.aizwys.cn

JS:   static f() {}
来源：http://kxb.zhixingplan.top

TS:   static f(): void {}
来源：http://fsp.snrcjt.cn

Java: static void f() {}
来源：http://sxl.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kas.yvedp.cn

Ruby: def self.f; end
来源：http://ygg.sufxvd.cn

C#:   public static void F() {}
来源：http://sch.xuanzx.com

[G09] 接口 / 抽象类
来源：http://cgv.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://atn.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jcn.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nun.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://dgj.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://lau.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://mtk.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ymg.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://ccn.yj20258888.top

[G10] 访问控制
来源：http://bws.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://ryy.snrcjt.cn

PHP:  public / protected / private
来源：http://bvx.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://qkv.smart0.xyz

TS:   public / protected / private
来源：http://mgq.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://jus.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://edz.ppjwa.cn

Ruby: public / protected / private
来源：http://xyi.guannengcc.top

C#:   public / protected / private / internal
来源：http://dwh.shuidangran.top

[G11] getter / setter
来源：http://mqj.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://zqw.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xuh.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://hqu.sufxvd.cn

TS:   get name(): string { return this._name; }
来源：http://zwc.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://ash.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uoa.vehdjk.com

Ruby: attr_accessor :name
来源：http://yii.daria6918.cn

C#:   public string Name { get; set; }
来源：http://ngb.ppjwa.cn

[G12] 对象转字符串
来源：http://hta.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://brg.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ntm.cucudq.cn

JS:   toString() { return this.name; }
来源：http://nsb.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://itq.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://anu.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ast.havefunace.top

Ruby: def to_s; @name; end
来源：http://mej.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://wlt.jinqigfzy.top

[G13] 判断对象类型
来源：http://hxs.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://qxs.nanxinkj.top

PHP:  $u instanceof User
来源：http://gef.bjfxy.top

JS:   u instanceof User
来源：http://jqp.zhengqikj.top

TS:   u instanceof User
来源：http://esa.zhijiandao.cn

Java: u instanceof User
来源：http://smm.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://bej.xinyue.icu

Ruby: u.is_a?(User)
来源：http://szo.xuanzx.com

C#:   u is User
来源：http://kyq.chenlongwang.top

[G14] 数据类 / record
来源：http://eoo.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jfk.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://cbw.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://eii.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://bwh.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://cbd.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://bjr.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fyk.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://nwe.jinqigufen.top

[G15] 枚举
来源：http://yit.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ytd.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mzv.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jix.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sff.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://qnj.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iab.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://gdq.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ubh.tanke756.top

[G16] 对象转数组 / 字典
来源：http://mdx.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ctd.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://ass.aibaodan.cn

JS:   Object.entries(obj)
来源：http://wnx.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://mzc.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://drr.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://svh.cdnleiting.top

Ruby: obj.instance_variables
来源：http://qud.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://klc.havefunace.top

================================================================================
来源：http://eom.nanxinkj.top

H. 异常与错误处理
来源：http://kog.iojbl.cn

================================================================================
来源：http://nln.mhx1999.top

[H01] try / catch 基础
来源：http://irv.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ijl.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fel.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ouh.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fin.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zoo.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rfn.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qzi.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uew.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://bgi.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://glr.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://imk.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tbr.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kkl.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://oza.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nge.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qqi.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sdw.hcnkem.com

[H03] 主动抛出异常
来源：http://jro.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://eoj.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gqe.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://cbs.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://cej.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://cvw.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fbd.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uio.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://rtm.yuxming.cn

[H04] 自定义异常类型
来源：http://pdr.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://wcg.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://yjb.316326.xyz

JS:   class MyError extends Error {}
来源：http://gvj.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://zmg.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://ywm.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fbo.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://eqs.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://xer.daxiang520.top

[H05] 捕获特定类型
来源：http://cou.316326.xyz

Py:   except ValueError as e:
来源：http://uxj.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xwf.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://emi.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://bym.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://cck.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://laj.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://uqq.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tmw.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://chv.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://ahn.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://egd.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://ffc.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yks.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://foa.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pkp.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://yql.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://div.zhoulong.xyz

[H07] 断言
来源：http://yfi.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://zgz.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://drc.bbcook.cn

JS:   console.assert(x > 0);
来源：http://cmk.bjfxy.top

TS:   console.assert(x > 0);
来源：http://tma.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://rkl.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bew.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yvp.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://gkc.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://hyb.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://mzp.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lcv.aizwys.cn

JS:   e.message;  e.stack
来源：http://hax.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://omk.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cbh.gaohongyu789.top

Go:   err.Error()
来源：http://mtn.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://vma.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://cff.bbcook.cn

[H09] 带错误码的异常
来源：http://php.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gla.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ndt.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sim.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vpc.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hfb.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cnz.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://gsn.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mcv.shuidangran.top

[H10] 资源自动释放
来源：http://bhw.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ynh.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pdq.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dic.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://phn.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vrq.yvedp.cn

Go:   defer f.Close()
来源：http://iwg.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ryu.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lgr.sweek.top

================================================================================
来源：http://jky.feifeiyinyue.top

I. 正则表达式
来源：http://gqa.hongshengwenyu.top

================================================================================
来源：http://lyz.hnqzz.top

[I01] 判断是否匹配
来源：http://ylv.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sjz.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://nlq.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://rdd.meibo888.top

TS:   /\d+/.test(s)
来源：http://ysr.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ult.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pwy.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://xcy.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ceu.yonumen.top

[I02] 提取所有匹配
来源：http://yly.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://wht.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://utk.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eav.cheryme.top

TS:   s.match(/\d+/g)
来源：http://xqh.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ptd.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rxn.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://vzi.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://udj.wangdashe.top

[I03] 提取捕获分组
来源：http://uow.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zyl.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hin.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://voz.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xav.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lju.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sbs.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://epc.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gas.gaohongyu789.top

[I04] 正则替换
来源：http://lye.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://omd.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tmb.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uqw.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://tjo.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://zdm.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tiu.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bts.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://smm.yonumen.top

[I05] 按正则拆分
来源：http://mft.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jas.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://imv.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://khc.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://rnf.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://eee.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lhn.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ilo.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://swh.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uss.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qkh.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zbi.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bjs.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dwe.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sol.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cmm.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xal.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mgo.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://vki.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eaw.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zei.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://onz.iojbl.cn

TS:   /error/gim
来源：http://hps.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lvd.tanke756.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aer.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://idp.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nhp.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://yhc.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mzz.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cmg.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gjl.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uxr.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qid.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gpc.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hkl.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kap.zhiwuduotai.top

================================================================================
来源：http://wvw.tianlin.xyz

J. 日期与时间
来源：http://fmd.zhengqikj.top

================================================================================
来源：http://unh.ydzc1.top

[J01] 获取当前时间
来源：http://pwd.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://old.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rmv.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://fyj.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://nfa.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yqr.yongpay.top


<!-- 参考信息 -->