代发 wailian999

Py:   class Admin(User): pass
来源：http://qtr.yonumen.top

PHP:  class Admin extends User {}
来源：http://awr.cheryme.top

JS:   class Admin extends User {}
来源：http://gxy.zdqjudy.top

TS:   class Admin extends User {}
来源：http://kzg.yj202588.top

Java: class Admin extends User {}
来源：http://ire.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lor.cheryme.top

Ruby: class Admin < User; end
来源：http://ayo.zhongyouzk.top

C#:   class Admin : User {}
来源：http://poj.tarul.cn

[G06] 重写方法
来源：http://zrn.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://bwd.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rkz.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://tcu.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://tmf.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://pfu.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aoi.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://btj.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://eay.cashguo.top

[G07] 调用父类方法
来源：http://iax.haohaochexian.top

Py:   super().greet()
来源：http://tcg.ctjpmb.com

PHP:  parent::greet();
来源：http://zjn.daria6918.cn

JS:   super.greet();
来源：http://ndb.iojbl.cn

TS:   super.greet();
来源：http://sjy.cqqwz.cn

Java: super.greet();
来源：http://mvt.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://edd.zhixingplan.top

Ruby: super
来源：http://kyt.cdnleiting.top

C#:   base.Greet();
来源：http://ujo.vehdjk.com

[G08] 静态方法与属性
来源：http://uef.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cgs.havefunace.top

PHP:  public static function f() {}
来源：http://cmw.haohaochexian.top

JS:   static f() {}
来源：http://yaq.hnxiangtu.top

TS:   static f(): void {}
来源：http://hby.svipenyu.cn

Java: static void f() {}
来源：http://yfb.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ara.zdqjudy.top

Ruby: def self.f; end
来源：http://lco.xylfe.cn

C#:   public static void F() {}
来源：http://fpz.cheryme.top

[G09] 接口 / 抽象类
来源：http://kal.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://hjf.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://lvm.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wsz.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://vvm.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://ygl.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://laa.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dzw.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://yvd.chenlongwang.top

[G10] 访问控制
来源：http://htw.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://lgx.xinyue.icu

PHP:  public / protected / private
来源：http://xna.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://fyk.birdmap.top

TS:   public / protected / private
来源：http://rae.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://zzl.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rxt.hesvh.cn

Ruby: public / protected / private
来源：http://bkk.smart0.xyz

C#:   public / protected / private / internal
来源：http://rfe.ywan-chungtsiang.top

[G11] getter / setter
来源：http://gqh.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://xgm.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://caa.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://fnt.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://tai.ehwqpu.com

Java: public String getName() { return name; }
来源：http://juy.xuanzx.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://iun.guowangkeji.top

Ruby: attr_accessor :name
来源：http://ack.xuanzx.com

C#:   public string Name { get; set; }
来源：http://rca.ydjk.org.cn

[G12] 对象转字符串
来源：http://qnj.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://lvr.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oyq.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://yqw.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://icj.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://tll.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://vnc.yfazqb.com

Ruby: def to_s; @name; end
来源：http://lgx.meibo888.top

C#:   public override string ToString() => Name;
来源：http://tsp.zhiwuduotai.top

[G13] 判断对象类型
来源：http://dii.shzxlz.cn

Py:   isinstance(u, User)
来源：http://lup.havefunace.top

PHP:  $u instanceof User
来源：http://wrc.zhiwuduotai.top

JS:   u instanceof User
来源：http://rqc.fktsv.cn

TS:   u instanceof User
来源：http://xvb.hnxiangtu.top

Java: u instanceof User
来源：http://hqt.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lab.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://xjn.hywenlv.cn

C#:   u is User
来源：http://twm.yueranfly.top

[G14] 数据类 / record
来源：http://gjm.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cua.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://rhv.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://xyh.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://iit.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://tkf.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://nyu.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sjy.ivvv.top

C#:   record User(string Name, int Age);
来源：http://wyp.vehdjk.com

[G15] 枚举
来源：http://bxm.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pem.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gzy.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pvr.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xvs.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://ilt.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fxl.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://ntx.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cvi.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://mdx.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bvi.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://iym.hfpthk.cn

JS:   Object.entries(obj)
来源：http://rtv.0kj1m.cn

TS:   Object.entries(obj)
来源：http://vld.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ied.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://iva.cqqwz.cn

Ruby: obj.instance_variables
来源：http://cky.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://zmi.yuanzhike.top

================================================================================
来源：http://yub.wangshuangyany.cn

H. 异常与错误处理
来源：http://paa.yuanzhike.top

================================================================================
来源：http://abe.zdbjq.cn

[H01] try / catch 基础
来源：http://dmd.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nei.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://odz.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qtx.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zwy.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wiq.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kbl.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://stp.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hoq.cucudq.cn

[H02] finally / ensure 收尾
来源：http://mow.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://gam.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tal.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://vpt.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lom.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ctl.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qnk.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://azl.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qbj.zhixingplan.top

[H03] 主动抛出异常
来源：http://pvv.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://emr.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zmf.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://jed.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://zgp.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ngl.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fyg.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yoc.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://upw.hnxiangtu.top

[H04] 自定义异常类型
来源：http://xpr.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://ewg.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://imk.xinyue.icu

JS:   class MyError extends Error {}
来源：http://exy.yuxming.cn

TS:   class MyError extends Error {}
来源：http://dph.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://tzx.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uqy.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://wch.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://muc.yuxming.cn

[H05] 捕获特定类型
来源：http://sxj.guowangkeji.top

Py:   except ValueError as e:
来源：http://mqt.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://laz.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://nrx.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://pzi.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://mjy.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wfr.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://vat.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jbk.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://yuc.fengsongda.top

Py:   value = d.get("k") or default
来源：http://auz.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://mcv.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gvu.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://yrc.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hvo.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qde.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://ixl.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://hml.guannengcc.top

[H07] 断言
来源：http://jwy.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://ukm.birdmap.top

PHP:  assert($x > 0);
来源：http://amu.meibo888.top

JS:   console.assert(x > 0);
来源：http://lwk.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://knn.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://tvh.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yjn.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://gss.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://xiy.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://oif.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://gus.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gow.hfpthk.cn

JS:   e.message;  e.stack
来源：http://uli.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bvm.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cez.hfpthk.cn

Go:   err.Error()
来源：http://uxh.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://ejg.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://wvi.yj20258.top

[H09] 带错误码的异常
来源：http://gme.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hta.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pes.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nrx.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mkq.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nbx.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://noy.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://qyi.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ohe.jinqigufen.top

[H10] 资源自动释放
来源：http://per.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tip.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://all.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jzu.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vsm.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vta.epnwcf.com

Go:   defer f.Close()
来源：http://ojc.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fli.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dac.fktsv.cn

================================================================================
来源：http://vvs.jinqigufen.top

I. 正则表达式
来源：http://cse.zhiwuduotai.top

================================================================================
来源：http://fot.cdnleiting.top

[I01] 判断是否匹配
来源：http://vhs.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://csq.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://qkp.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://hak.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://gzq.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nyb.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cax.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://lex.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hkk.jinqigufen.top

[I02] 提取所有匹配
来源：http://zxv.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://ezd.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://phi.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qxo.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://tkv.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uvo.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ena.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://gsu.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hla.jqgufenzy.top

[I03] 提取捕获分组
来源：http://jpq.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jxa.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jlt.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jmu.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hmn.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lak.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://awz.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ulj.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lnl.ydzc1.top

[I04] 正则替换
来源：http://dty.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nlp.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://osj.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ycg.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://kcr.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://vpf.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qbo.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gog.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vbb.wangdashe.top

[I05] 按正则拆分
来源：http://gsc.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pml.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oba.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ofz.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://bcq.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://eqb.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nms.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mrr.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ucs.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ept.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vxh.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://adi.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ely.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cik.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qyo.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://idx.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zwe.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gho.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://sty.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mat.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ipn.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rzb.aibaodan.cn

TS:   /error/gim
来源：http://oii.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tzm.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ovf.uphjek.com

Ruby: s.scan(/error/i)
来源：http://fay.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oqh.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://vks.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fda.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rjo.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://loj.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://imv.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oon.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eyj.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpa.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wsl.havefunace.top

================================================================================
来源：http://axc.mhx1999.top

J. 日期与时间
来源：http://bst.fktsv.cn

================================================================================
来源：http://rjm.cheryme.top

[J01] 获取当前时间
来源：http://yho.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://toy.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qqg.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://stq.sysykeji.top

TS:   new Date();  Date.now()
来源：http://nip.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qgd.iojbl.cn

Go:   time.Now()
来源：http://vmq.yonumen.top

Ruby: Time.now
来源：http://cpt.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dfz.fzhhl.top

[J02] 格式化输出
来源：http://uzy.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gcz.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://arl.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kts.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://eez.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zje.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bdc.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wdh.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dyl.0kj1m.cn

[J03] 字符串解析为日期
来源：http://lfn.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dlp.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://byb.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://rxd.haohaochexian.top


<!-- 参考信息 -->