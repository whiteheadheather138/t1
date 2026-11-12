代发 wailian999

JS:   this.name = "x";
来源：http://our.sxryk.cn

TS:   name: string = "x";
来源：http://qid.fktsv.cn

Java: private String name;
来源：http://mwo.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fxn.smart0.xyz

Ruby: @name = "x"
来源：http://gbd.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://qrp.chenjidiqi.icu

[G04] 定义方法
来源：http://cxx.yfazqb.com

Py:   def greet(self): return self.name
来源：http://vkd.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fic.yueranfly.top

JS:   greet() { return this.name; }
来源：http://mbv.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://kgu.hfpthk.cn

Java: String greet() { return name; }
来源：http://aud.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://tkf.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://ljc.yj20258888.top

C#:   public string Greet() => Name;
来源：http://jgq.sxryk.cn

[G05] 继承
来源：http://ets.tianlin.xyz

Py:   class Admin(User): pass
来源：http://amd.andypj.xyz

PHP:  class Admin extends User {}
来源：http://edk.snrcjt.cn

JS:   class Admin extends User {}
来源：http://hha.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://ygm.zhijiandao.cn

Java: class Admin extends User {}
来源：http://dbi.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tkv.gzhubu.top

Ruby: class Admin < User; end
来源：http://izs.gotoacloud.top

C#:   class Admin : User {}
来源：http://tbp.jinqigfzy.top

[G06] 重写方法
来源：http://nvp.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://uxh.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://esu.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://mix.fengsongda.top

TS:   greet(): string { return "admin"; }
来源：http://tcv.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://giv.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://env.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://mla.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://mtu.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://rky.yanxiufei.cn

Py:   super().greet()
来源：http://soh.yonumen.top

PHP:  parent::greet();
来源：http://rzl.yonumen.top

JS:   super.greet();
来源：http://pij.shanyushiyangkeji.top

TS:   super.greet();
来源：http://vbg.meibo888.top

Java: super.greet();
来源：http://gqs.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lmy.sjlbkw.cn

Ruby: super
来源：http://jpe.daria6918.cn

C#:   base.Greet();
来源：http://tvl.redwolf501.top

[G08] 静态方法与属性
来源：http://aul.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nhe.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://hai.tarul.cn

JS:   static f() {}
来源：http://yqc.svipenyu.cn

TS:   static f(): void {}
来源：http://cqh.guowangkeji.top

Java: static void f() {}
来源：http://azj.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vmd.fengsongda.top

Ruby: def self.f; end
来源：http://iba.wangdashe.top

C#:   public static void F() {}
来源：http://bzs.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://tfm.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://yjf.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://tky.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xth.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://zfs.nwbrower.top

Java: interface Shape { double area(); }
来源：http://dor.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://bmr.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://btg.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://kwq.hnqzz.top

[G10] 访问控制
来源：http://avj.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://qmv.jiagoushi.top

PHP:  public / protected / private
来源：http://yfg.cheryme.top

JS:   #private 字段；其余公开
来源：http://qre.zhoulong.xyz

TS:   public / protected / private
来源：http://fgq.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://sxs.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kdz.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://uhl.ivvv.top

C#:   public / protected / private / internal
来源：http://wvk.fzhhl.top

[G11] getter / setter
来源：http://gyo.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://tpm.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vuz.tanke756.top

JS:   get name() { return this._name; }
来源：http://pea.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://mqy.cucudq.cn

Java: public String getName() { return name; }
来源：http://tae.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qqc.yj202588.top

Ruby: attr_accessor :name
来源：http://lgl.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://vth.jyoumei.cn

[G12] 对象转字符串
来源：http://hyb.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://gay.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://cut.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://hjj.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://jph.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://byo.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hau.xinyue.icu

Ruby: def to_s; @name; end
来源：http://pod.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://nur.sweek.top

[G13] 判断对象类型
来源：http://pzk.pycfn.com

Py:   isinstance(u, User)
来源：http://vbb.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://evp.chenzaomai.com

JS:   u instanceof User
来源：http://njr.ppjwa.cn

TS:   u instanceof User
来源：http://ylf.birdmap.top

Java: u instanceof User
来源：http://tob.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ijq.hcnkem.com

Ruby: u.is_a?(User)
来源：http://xkn.hnxiangtu.top

C#:   u is User
来源：http://hxz.birdmap.top

[G14] 数据类 / record
来源：http://iai.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ckh.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://gqw.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ypk.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://awv.havefunace.top

Java: record User(String name, int age) {}
来源：http://vtr.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://nnf.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zfe.tanke756.top

C#:   record User(string Name, int Age);
来源：http://jvb.tianlin.xyz

[G15] 枚举
来源：http://kfc.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uos.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lqi.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cci.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jfc.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://sml.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zav.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://uvf.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jza.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://dtg.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cit.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://yfm.epnwcf.com

JS:   Object.entries(obj)
来源：http://zkv.shzxlz.cn

TS:   Object.entries(obj)
来源：http://aen.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nnj.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xsq.nwbrower.top

Ruby: obj.instance_variables
来源：http://oqx.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://jmm.yj20258.top

================================================================================
来源：http://lrt.fehbvm.com

H. 异常与错误处理
来源：http://ubo.shangyingyoupin.top

================================================================================
来源：http://uhp.nanxuanxn.top

[H01] try / catch 基础
来源：http://whg.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qjm.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mvr.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ffw.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uxm.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uqw.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vrg.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xoh.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ywe.havefunace.top

[H02] finally / ensure 收尾
来源：http://nfr.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://sfa.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kom.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bun.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bjp.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tzk.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xxe.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ixu.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wlp.yj202588.top

[H03] 主动抛出异常
来源：http://dky.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://rcq.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vje.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://ojw.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://xun.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ndm.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tfb.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://owa.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://luv.hnqzz.top

[H04] 自定义异常类型
来源：http://xvt.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://dvc.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cof.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://xri.c1oappe.top

TS:   class MyError extends Error {}
来源：http://rrn.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://wsm.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://obr.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://niu.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://kys.aibaodan.cn

[H05] 捕获特定类型
来源：http://ssk.zycfv.cn

Py:   except ValueError as e:
来源：http://hvx.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://acq.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://nfb.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://bbu.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://qac.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nme.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://lfd.jiagoushi.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fko.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://jpi.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://oqv.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eqh.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://rjq.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://cde.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xwf.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://brq.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://wav.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://wti.wangshuangyany.cn

[H07] 断言
来源：http://ega.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://boo.wangdashe.top

PHP:  assert($x > 0);
来源：http://vgq.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://pqi.vehdjk.com

TS:   console.assert(x > 0);
来源：http://bav.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://pwn.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tee.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://hfh.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://mcy.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://dhg.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://uku.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jvz.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://tyb.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pue.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ibj.daxiang520.top

Go:   err.Error()
来源：http://xfq.sweek.top

Ruby: e.message;  e.backtrace
来源：http://vvu.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://gpa.vqdsnc.cn

[H09] 带错误码的异常
来源：http://jdz.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://als.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yqg.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aar.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bqy.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fzc.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://snj.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mhr.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sam.cqqwz.cn

[H10] 资源自动释放
来源：http://wqr.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yyk.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dik.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dcy.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pvi.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgk.epnwcf.com

Go:   defer f.Close()
来源：http://eqz.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pvd.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xik.pycfn.com

================================================================================
来源：http://zco.smart0.xyz

I. 正则表达式
来源：http://mpm.jinqigfzy.top

================================================================================
来源：http://qdu.hnqzz.top

[I01] 判断是否匹配
来源：http://ybx.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ach.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qsc.yvedp.cn

JS:   /\d+/.test(s)
来源：http://vmp.nwbrower.top

TS:   /\d+/.test(s)
来源：http://xqm.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pje.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://byo.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://oop.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bih.tian-w.cn

[I02] 提取所有匹配
来源：http://zdo.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://hoh.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qjz.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ifp.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://nvd.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://swf.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kyu.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://kei.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ela.yj20258888.top

[I03] 提取捕获分组
来源：http://knu.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nmf.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://isq.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://egn.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cec.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vuj.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://etk.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iso.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tra.quarkkingdee.top

[I04] 正则替换
来源：http://usl.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jtp.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yoc.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://pse.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://pfi.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://kek.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gss.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hyp.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bgu.hcnkem.com

[I05] 按正则拆分
来源：http://vyc.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://akv.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qxu.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ydy.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://nyz.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://egy.hywenlv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://key.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://uzm.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xmm.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ase.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qry.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://egc.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jlj.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xiz.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rhz.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sxb.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xfi.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kpt.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://lrr.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ydf.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbm.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://stp.dashuyun.cn

TS:   /error/gim
来源：http://jsy.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tyy.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://brt.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://rig.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lhv.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://lzc.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kui.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xys.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blu.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ptn.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iuu.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gqu.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kje.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rzt.dashuyun.cn

================================================================================
来源：http://qff.ydjk.org.cn

J. 日期与时间
来源：http://dzz.hywenlv.cn

================================================================================
来源：http://ipn.xinyue.icu

[J01] 获取当前时间
来源：http://piv.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://tdj.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ret.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://ikw.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://cgm.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ixm.cdnleiting.top


<!-- 参考信息 -->