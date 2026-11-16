代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://kvr.shzxlz.cn

[G03] 实例属性
来源：http://ycb.jinqigfzy.top

Py:   self.name = "x"
来源：http://twt.316326.xyz

PHP:  public string $name = "x";
来源：http://dnl.sxryk.cn

JS:   this.name = "x";
来源：http://hbq.cqqwz.cn

TS:   name: string = "x";
来源：http://ewu.shzxlz.cn

Java: private String name;
来源：http://kgv.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qdj.gotoacloud.top

Ruby: @name = "x"
来源：http://tnb.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://tcl.gotoacloud.top

[G04] 定义方法
来源：http://cpk.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://aug.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://thz.guannengcc.top

JS:   greet() { return this.name; }
来源：http://gws.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://kgf.xuanzx.com

Java: String greet() { return name; }
来源：http://aoz.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hba.epnwcf.com

Ruby: def greet; @name; end
来源：http://tdr.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://bjr.zhoulong.xyz

[G05] 继承
来源：http://lcy.meibo888.top

Py:   class Admin(User): pass
来源：http://zee.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://sri.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://byb.jyoumei.cn

TS:   class Admin extends User {}
来源：http://ney.hnqzz.top

Java: class Admin extends User {}
来源：http://kha.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtv.gogol.net.cn

Ruby: class Admin < User; end
来源：http://pmm.jyoumei.cn

C#:   class Admin : User {}
来源：http://bib.xuetiantiany.cn

[G06] 重写方法
来源：http://xhf.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://imx.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vrn.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://yoy.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://rpu.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://xsf.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sci.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://tip.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://lmy.tian-w.cn

[G07] 调用父类方法
来源：http://wmq.aibaodan.cn

Py:   super().greet()
来源：http://whb.yuxming.cn

PHP:  parent::greet();
来源：http://iou.tian-w.cn

JS:   super.greet();
来源：http://ytz.tian-w.cn

TS:   super.greet();
来源：http://fjh.nanxuanxn.top

Java: super.greet();
来源：http://jra.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pux.gotoacloud.top

Ruby: super
来源：http://ceg.zhengqikj.top

C#:   base.Greet();
来源：http://ukl.yangfankeji.com

[G08] 静态方法与属性
来源：http://txc.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bqc.hysaishi.cn

PHP:  public static function f() {}
来源：http://gny.redwolf501.top

JS:   static f() {}
来源：http://wrm.sweek.top

TS:   static f(): void {}
来源：http://vah.jqgfzy.top

Java: static void f() {}
来源：http://gld.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ecn.wangshuangyany.cn

Ruby: def self.f; end
来源：http://nno.haohaochexian.top

C#:   public static void F() {}
来源：http://npe.fktsv.cn

[G09] 接口 / 抽象类
来源：http://hse.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://ycz.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mgq.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://klj.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://yce.jianghu66.top

Java: interface Shape { double area(); }
来源：http://voy.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://dji.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fbx.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://cvr.shzxlz.cn

[G10] 访问控制
来源：http://qda.smart0.xyz

Py:   约定 _protected / __private（不强制）
来源：http://amu.shuidangran.top

PHP:  public / protected / private
来源：http://nup.c1oappe.top

JS:   #private 字段；其余公开
来源：http://caf.meibo888.top

TS:   public / protected / private
来源：http://wvs.gogol.net.cn

Java: public / protected / private / 默认包级
来源：http://xld.tanke756.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mot.zdqjudy.top

Ruby: public / protected / private
来源：http://huy.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://eou.andypj.xyz

[G11] getter / setter
来源：http://stw.jianghu66.top

Py:   @property 与 @x.setter
来源：http://ksx.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yrz.epnwcf.com

JS:   get name() { return this._name; }
来源：http://blp.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://bbe.sxryk.cn

Java: public String getName() { return name; }
来源：http://klo.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xdx.haohaochexian.top

Ruby: attr_accessor :name
来源：http://hks.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://cem.ivvv.top

[G12] 对象转字符串
来源：http://wrb.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://mxx.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://quk.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://trn.sweek.top

TS:   toString(): string { return this.name; }
来源：http://thx.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://ays.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://gkg.tian-w.cn

Ruby: def to_s; @name; end
来源：http://hsk.yj20258.top

C#:   public override string ToString() => Name;
来源：http://ttb.havefunace.top

[G13] 判断对象类型
来源：http://gis.gogol.net.cn

Py:   isinstance(u, User)
来源：http://yhp.hnqzz.top

PHP:  $u instanceof User
来源：http://aiv.birdmap.top

JS:   u instanceof User
来源：http://fxt.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://fdy.sysykeji.top

Java: u instanceof User
来源：http://qav.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bdt.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://dxc.vqdsnc.cn

C#:   u is User
来源：http://qkb.yanxiufei.cn

[G14] 数据类 / record
来源：http://ecw.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wcb.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://jow.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wys.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://sfl.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://jvj.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://xxq.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://czx.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://lii.snrcjt.cn

[G15] 枚举
来源：http://zzc.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mrg.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vil.sjlbkw.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dmp.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jje.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://kip.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://len.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://clf.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zhd.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://qmh.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gwo.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://lrl.52xcode.cn

JS:   Object.entries(obj)
来源：http://ryq.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://aeb.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rkm.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ktn.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://wit.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://wil.zdbjq.cn

================================================================================
来源：http://lux.52xcode.cn

H. 异常与错误处理
来源：http://wpj.ppjwa.cn

================================================================================
来源：http://ryf.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://bnb.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zbe.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://siy.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gtw.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gbp.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fxz.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tzz.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dju.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ywc.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://usa.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://vgp.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hep.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hss.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pue.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://cvd.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cmp.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pti.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jbz.fehbvm.com

[H03] 主动抛出异常
来源：http://chy.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://vvl.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eiw.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://isg.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://vyd.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://hkz.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://owv.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vyr.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://ctn.yvedp.cn

[H04] 自定义异常类型
来源：http://ruj.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://bkr.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://yxc.iojbl.cn

JS:   class MyError extends Error {}
来源：http://acz.xylfe.cn

TS:   class MyError extends Error {}
来源：http://mkj.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://gge.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bef.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://eaw.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://gjc.sjlbkw.cn

[H05] 捕获特定类型
来源：http://kbx.yvedp.cn

Py:   except ValueError as e:
来源：http://jrw.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://msx.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://hyn.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://tku.wangdashe.top

Java: catch (IOException | SQLException e) {}
来源：http://vby.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hce.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://avk.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wlm.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://iwb.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://dsx.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://gpq.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://lxp.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://msb.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ybg.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sfu.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://dti.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://hyo.chenjidiqi.icu

[H07] 断言
来源：http://zlv.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://jpu.cdnleiting.top

PHP:  assert($x > 0);
来源：http://bqs.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://acw.zycfv.cn

TS:   console.assert(x > 0);
来源：http://kig.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://ljs.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vmx.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://bdx.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://mxw.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://znm.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://awp.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vrn.jianghu66.top

JS:   e.message;  e.stack
来源：http://zug.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tze.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qij.hfpthk.cn

Go:   err.Error()
来源：http://bdb.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://dwd.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://zna.snrcjt.cn

[H09] 带错误码的异常
来源：http://muo.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bgy.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wgo.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kuo.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdr.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://icl.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://utn.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://aiw.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xbd.sysykeji.top

[H10] 资源自动释放
来源：http://xev.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lph.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rin.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qmu.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nzw.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tsi.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://afe.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ebm.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dqw.yuxming.cn

================================================================================
来源：http://vtt.dashuyun.cn

I. 正则表达式
来源：http://izo.yuxming.cn

================================================================================
来源：http://wew.uphjek.com

[I01] 判断是否匹配
来源：http://dau.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://saj.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://jgw.cucudq.cn

JS:   /\d+/.test(s)
来源：http://nqb.mhx1999.top

TS:   /\d+/.test(s)
来源：http://mtl.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hho.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ljf.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://hrc.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nxj.iojbl.cn

[I02] 提取所有匹配
来源：http://jnv.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://klp.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hpe.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ncl.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://zse.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tyo.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ihm.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://amj.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tez.cucudq.cn

[I03] 提取捕获分组
来源：http://anb.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tzf.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rtj.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rru.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zww.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://idl.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cxx.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zuv.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://guy.ybcxt.top

[I04] 正则替换
来源：http://ryt.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sms.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lvq.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://zcd.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://kok.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://lrw.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hqn.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rhm.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ghu.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://bfu.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://shv.chenjidiqi.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qbi.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://uyr.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://ebd.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://zdt.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zhv.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://wll.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eyl.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://agk.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oxv.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nzw.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ljg.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://klp.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yet.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://foq.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zgb.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lhx.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://pwh.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tit.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hsw.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lmv.dashuyun.cn

TS:   /error/gim
来源：http://mrc.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pbb.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yxl.yonumen.top

Ruby: s.scan(/error/i)
来源：http://uwv.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://loo.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://emd.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uij.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gyu.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljo.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ceu.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lyn.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rgt.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cph.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kgn.ehwqpu.com

================================================================================
来源：http://exs.snrcjt.cn

J. 日期与时间
来源：http://zlm.pycfn.com

================================================================================
来源：http://cuc.c1oappe.top

[J01] 获取当前时间
来源：http://ypy.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ulz.wangdashe.top


<!-- 参考信息 -->