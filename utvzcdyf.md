代发 wailian999

Java: class Admin extends User {}
来源：http://lvu.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qgq.tarul.cn

Ruby: class Admin < User; end
来源：http://hom.zhongyouzk.top

C#:   class Admin : User {}
来源：http://afm.jinqigufen.top

[G06] 重写方法
来源：http://oxl.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://web.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cbx.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://jhe.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://zhy.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://nmd.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jfj.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://snl.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://rgk.yj202588.top

[G07] 调用父类方法
来源：http://sxx.yuxming.cn

Py:   super().greet()
来源：http://qdf.316326.xyz

PHP:  parent::greet();
来源：http://rlf.vqdsnc.cn

JS:   super.greet();
来源：http://czg.jianghu66.top

TS:   super.greet();
来源：http://plx.zhiwuduotai.top

Java: super.greet();
来源：http://odo.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rha.sufxvd.cn

Ruby: super
来源：http://pzb.yonumen.top

C#:   base.Greet();
来源：http://ieb.fzhhl.top

[G08] 静态方法与属性
来源：http://pfm.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://otj.gogol.net.cn

PHP:  public static function f() {}
来源：http://fwa.tarul.cn

JS:   static f() {}
来源：http://hhm.xziqi.cn

TS:   static f(): void {}
来源：http://rix.aibaodan.cn

Java: static void f() {}
来源：http://anm.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aqy.hongshengwenyu.top

Ruby: def self.f; end
来源：http://jrk.bjfxy.top

C#:   public static void F() {}
来源：http://cwr.hcnkem.com

[G09] 接口 / 抽象类
来源：http://tev.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://lrp.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://bbl.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhc.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://isw.cheryme.top

Java: interface Shape { double area(); }
来源：http://rkk.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://yqc.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rnw.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://kur.yuxming.cn

[G10] 访问控制
来源：http://uaq.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://fns.uphjek.com

PHP:  public / protected / private
来源：http://ayl.xuanzx.com

JS:   #private 字段；其余公开
来源：http://yho.bjfxy.top

TS:   public / protected / private
来源：http://pwo.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://jhh.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rkp.quarkkingdee.top

Ruby: public / protected / private
来源：http://jog.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://dno.9152youxi.cn

[G11] getter / setter
来源：http://vex.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://jnw.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://cah.fktsv.cn

JS:   get name() { return this._name; }
来源：http://sem.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://ipn.smart0.xyz

Java: public String getName() { return name; }
来源：http://mfi.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://hut.daria6918.cn

Ruby: attr_accessor :name
来源：http://rhe.xuanzx.com

C#:   public string Name { get; set; }
来源：http://coz.hcnkem.com

[G12] 对象转字符串
来源：http://akr.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://fma.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dyk.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://cpa.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://cod.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://aae.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ozl.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://xru.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://ykm.guannengcc.top

[G13] 判断对象类型
来源：http://mxa.gogol.net.cn

Py:   isinstance(u, User)
来源：http://plz.xinyue.icu

PHP:  $u instanceof User
来源：http://yhr.fktsv.cn

JS:   u instanceof User
来源：http://lfn.guannengcc.top

TS:   u instanceof User
来源：http://yex.hnxiangtu.top

Java: u instanceof User
来源：http://gcs.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hmn.hesvh.cn

Ruby: u.is_a?(User)
来源：http://fus.jinqigfzy.top

C#:   u is User
来源：http://bgb.xuanzx.com

[G14] 数据类 / record
来源：http://cvf.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gup.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://kkp.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fwm.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://nuy.haohaochexian.top

Java: record User(String name, int age) {}
来源：http://cxa.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://chm.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yrn.sweek.top

C#:   record User(string Name, int Age);
来源：http://ray.yuxming.cn

[G15] 枚举
来源：http://zoe.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pru.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jta.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hsw.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eiq.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://edj.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://afx.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://dld.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tyb.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://abs.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hjj.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://orp.chenlongwang.top

JS:   Object.entries(obj)
来源：http://qvl.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://kpv.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lpu.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xcz.cdnleiting.top

Ruby: obj.instance_variables
来源：http://wud.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://val.yj20258.top

================================================================================
来源：http://ahn.yj20258888.top

H. 异常与错误处理
来源：http://roj.yj20258888.top

================================================================================
来源：http://djc.c1oappe.top

[H01] try / catch 基础
来源：http://vrl.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jzy.pengpengdd.cyou

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vnh.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pfy.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jhg.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cel.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pwn.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ewi.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ibx.yonumen.top

[H02] finally / ensure 收尾
来源：http://tyg.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eqx.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jfx.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sfo.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qgs.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://jwa.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ywp.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ojz.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tpb.jyoumei.cn

[H03] 主动抛出异常
来源：http://oyx.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://mlt.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wuy.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://iwz.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://wxz.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ige.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ckx.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qrq.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://udq.jlsjyb.cn

[H04] 自定义异常类型
来源：http://raj.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://okw.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://hzp.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://bel.iojbl.cn

TS:   class MyError extends Error {}
来源：http://uuy.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://lhn.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ekn.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://jij.iojbl.cn

C#:   class MyException : Exception {}
来源：http://sjl.andypj.xyz

[H05] 捕获特定类型
来源：http://vzb.yonumen.top

Py:   except ValueError as e:
来源：http://ezm.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uwi.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://osm.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://mgd.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://gyi.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hvg.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://vpq.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://woz.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://xcy.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://xex.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://ceo.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://vuj.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://jno.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://adr.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ifd.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://qyi.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://rid.sjlbkw.cn

[H07] 断言
来源：http://yys.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://wlv.guowangkeji.top

PHP:  assert($x > 0);
来源：http://ykn.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://zwy.yueranfly.top

TS:   console.assert(x > 0);
来源：http://ool.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://iiw.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fyj.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://wct.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://pob.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://stp.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://qtd.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://puc.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://qvo.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vjo.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://osd.cdnleiting.top

Go:   err.Error()
来源：http://smn.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://kch.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://hps.birdmap.top

[H09] 带错误码的异常
来源：http://lgo.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xnj.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://blo.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tdc.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwu.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://itj.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mgb.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cjx.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mkw.jianghu66.top

[H10] 资源自动释放
来源：http://hek.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fnf.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wpm.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qsy.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qeg.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://djo.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://hjd.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lyf.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vbs.gzhubu.top

================================================================================
来源：http://brg.havefunace.top

I. 正则表达式
来源：http://zvw.52xcode.cn

================================================================================
来源：http://wdw.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://usm.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pmo.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://wcj.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://kph.sysykeji.top

TS:   /\d+/.test(s)
来源：http://gfu.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yot.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://suh.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://bqb.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mva.tanke756.top

[I02] 提取所有匹配
来源：http://emx.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://jgi.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xuu.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oly.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://hrz.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tie.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eym.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://uvx.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dsm.ehwqpu.com

[I03] 提取捕获分组
来源：http://mot.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://scj.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rzj.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aak.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://teo.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ciy.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://feq.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pio.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xgj.haohaochexian.top

[I04] 正则替换
来源：http://tba.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nft.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uem.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://ylb.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://nfh.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://oym.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://izd.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uoo.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://evj.epnwcf.com

[I05] 按正则拆分
来源：http://shm.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xci.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mzh.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://yye.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://hgh.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://cic.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ylr.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://duq.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dyt.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ytf.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wpa.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gmg.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rti.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zmc.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://srq.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vcg.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qwo.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://usz.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://gtg.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bwx.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yqm.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lhl.jinghuilouyu.cn

TS:   /error/gim
来源：http://xgf.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yds.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://des.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://qbm.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://too.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://vyb.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://orz.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://psg.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://emh.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pun.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ztc.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aty.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mel.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qlq.jyoumei.cn

================================================================================
来源：http://xwr.bbcook.cn

J. 日期与时间
来源：http://kor.jinyuanbaomall.cn

================================================================================
来源：http://kly.pengpengdd.cyou

[J01] 获取当前时间
来源：http://ghz.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://tfb.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ctp.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://ywf.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://lzh.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vdv.wangshuangyany.cn

Go:   time.Now()
来源：http://qav.epnwcf.com

Ruby: Time.now
来源：http://byd.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nit.0kj1m.cn

[J02] 格式化输出
来源：http://hgi.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qlh.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://txw.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rik.zdbjq.cn

TS:   d.toISOString()
来源：http://akc.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gpd.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xur.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vvq.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://coc.ppjwa.cn

[J03] 字符串解析为日期
来源：http://nyp.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://awf.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hjg.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://iyv.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://vbc.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://tpw.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://duc.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://sru.sufxvd.cn


<!-- 参考信息 -->