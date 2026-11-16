代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://rvj.zycfv.cn

Ruby: def greet; @name; end
来源：http://tcj.yonumen.top

C#:   public string Greet() => Name;
来源：http://gqt.jqgufenzy.top

[G05] 继承
来源：http://rvs.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://kcy.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://vme.yvedp.cn

JS:   class Admin extends User {}
来源：http://lzp.sysykeji.top

TS:   class Admin extends User {}
来源：http://pxr.kuanghao11.cn

Java: class Admin extends User {}
来源：http://aol.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wgs.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://awu.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://nvp.yvedp.cn

[G06] 重写方法
来源：http://qrg.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://sow.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://shc.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://jhr.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://uup.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://dil.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crm.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://exq.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://uwu.birdmap.top

[G07] 调用父类方法
来源：http://zne.jianghu66.top

Py:   super().greet()
来源：http://ths.feifeiyinyue.top

PHP:  parent::greet();
来源：http://zou.jianghu66.top

JS:   super.greet();
来源：http://sbn.cqqwz.cn

TS:   super.greet();
来源：http://rcz.ppjwa.cn

Java: super.greet();
来源：http://eju.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kjp.jinyuanbaomall.cn

Ruby: super
来源：http://aje.tarul.cn

C#:   base.Greet();
来源：http://mnn.cashguo.top

[G08] 静态方法与属性
来源：http://jir.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rpc.daria6918.cn

PHP:  public static function f() {}
来源：http://tbv.redwolf501.top

JS:   static f() {}
来源：http://omn.guowangkeji.top

TS:   static f(): void {}
来源：http://tzy.yuxming.cn

Java: static void f() {}
来源：http://mac.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jkd.nwbrower.top

Ruby: def self.f; end
来源：http://phw.gogol.net.cn

C#:   public static void F() {}
来源：http://dba.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://mpd.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://two.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://cjw.hesvh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kon.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://fvx.gzhubu.top

Java: interface Shape { double area(); }
来源：http://uml.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://ymd.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://inz.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://bip.sjlbkw.cn

[G10] 访问控制
来源：http://oqy.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://lee.meibo888.top

PHP:  public / protected / private
来源：http://zij.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://ldj.iojbl.cn

TS:   public / protected / private
来源：http://xxk.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://mnm.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://drt.svipenyu.cn

Ruby: public / protected / private
来源：http://rrd.xinyue.icu

C#:   public / protected / private / internal
来源：http://eke.jianghu66.top

[G11] getter / setter
来源：http://hrr.uphjek.com

Py:   @property 与 @x.setter
来源：http://pjg.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://oib.c1oappe.top

JS:   get name() { return this._name; }
来源：http://yea.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://vvi.tanke756.top

Java: public String getName() { return name; }
来源：http://leq.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dvd.jyoumei.cn

Ruby: attr_accessor :name
来源：http://yri.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://ubk.hnqzz.top

[G12] 对象转字符串
来源：http://vpj.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://fni.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xgu.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://spi.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://ngr.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://hdy.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qid.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://abl.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://omc.redwolf501.top

[G13] 判断对象类型
来源：http://ztl.zdbjq.cn

Py:   isinstance(u, User)
来源：http://wmr.dianchejie.cn

PHP:  $u instanceof User
来源：http://cxy.yonumen.top

JS:   u instanceof User
来源：http://gzs.pengpengdd.cyou

TS:   u instanceof User
来源：http://pkm.haohaochexian.top

Java: u instanceof User
来源：http://dvj.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://toy.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://yny.havefunace.top

C#:   u is User
来源：http://bvm.jlsjyb.cn

[G14] 数据类 / record
来源：http://tjq.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gqr.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://yzq.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lwy.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://zev.hnqzz.top

Java: record User(String name, int age) {}
来源：http://gak.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://bzy.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ekz.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://oku.vqdsnc.cn

[G15] 枚举
来源：http://oft.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tub.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vhi.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ogc.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mht.sweek.top

Java: enum Color { RED, GREEN }
来源：http://itm.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xsd.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://bme.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qst.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://rco.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://slg.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://gav.dashuyun.cn

JS:   Object.entries(obj)
来源：http://qfv.ctjpmb.com

TS:   Object.entries(obj)
来源：http://uuo.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lat.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hst.daxiang520.top

Ruby: obj.instance_variables
来源：http://mwl.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://cke.zhaomingkeji.xyz

================================================================================
来源：http://zkm.epnwcf.com

H. 异常与错误处理
来源：http://ukk.52xcode.cn

================================================================================
来源：http://tma.shuidangran.top

[H01] try / catch 基础
来源：http://lnh.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ibr.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xlg.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zzq.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wrx.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uhu.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dya.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://weh.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tnq.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://iqh.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://bwe.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ikh.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qjj.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://arr.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://gyq.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nad.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sef.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://suc.0kj1m.cn

[H03] 主动抛出异常
来源：http://zfd.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://jkk.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hdr.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://ffm.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://gyl.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://snh.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uik.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kld.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://mlq.52xcode.cn

[H04] 自定义异常类型
来源：http://hvv.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://iqq.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aqd.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://nws.xuanzx.com

TS:   class MyError extends Error {}
来源：http://lsn.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://fwt.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://akh.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://cdv.c1oappe.top

C#:   class MyException : Exception {}
来源：http://htq.ydzc1.top

[H05] 捕获特定类型
来源：http://yxr.wangdashe.top

Py:   except ValueError as e:
来源：http://vum.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jdf.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://eul.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://ufa.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://cjd.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cfq.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://rnv.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oek.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://dmt.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://esv.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eol.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://kwd.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://mti.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tux.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://urw.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://orz.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://qro.tarul.cn

[H07] 断言
来源：http://rbs.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://zhs.ctjpmb.com

PHP:  assert($x > 0);
来源：http://qev.xuanzx.com

JS:   console.assert(x > 0);
来源：http://flm.epnwcf.com

TS:   console.assert(x > 0);
来源：http://qdy.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://omz.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://haa.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://why.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://uea.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://ysv.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://ael.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zry.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://qch.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ytz.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dwy.0kj1m.cn

Go:   err.Error()
来源：http://tqb.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://zek.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://xtv.zdqjudy.top

[H09] 带错误码的异常
来源：http://aly.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gdt.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://har.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://the.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qlv.cashguo.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ubj.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yef.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://tum.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://avo.tian-w.cn

[H10] 资源自动释放
来源：http://nvg.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xos.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zzw.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xtt.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xqz.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fzv.0kj1m.cn

Go:   defer f.Close()
来源：http://ocm.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tal.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://edx.iojbl.cn

================================================================================
来源：http://dqr.sweek.top

I. 正则表达式
来源：http://tmf.daria6918.cn

================================================================================
来源：http://ofv.aizwys.cn

[I01] 判断是否匹配
来源：http://ehs.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qxe.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fqj.tian-w.cn

JS:   /\d+/.test(s)
来源：http://dus.gzhubu.top

TS:   /\d+/.test(s)
来源：http://ure.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://giv.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ioo.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://vcq.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wab.meibo888.top

[I02] 提取所有匹配
来源：http://yug.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://nfc.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ory.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uwr.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://wvx.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rof.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kts.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://eks.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fgj.cqqwz.cn

[I03] 提取捕获分组
来源：http://smi.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://deb.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hcr.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hez.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lyz.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://boj.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cmb.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wpt.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yjy.jinqigfzy.top

[I04] 正则替换
来源：http://kzc.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ovm.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://npx.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://ron.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://mxf.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://blp.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rjo.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://blg.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hca.uphjek.com

[I05] 按正则拆分
来源：http://uoc.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qky.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tsn.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://fwf.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://nra.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://htj.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hbc.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://uro.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wjx.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kdi.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tpa.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fvy.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://okl.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://byi.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xit.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ejf.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ipy.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vbo.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://reo.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ntr.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bjj.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qyk.xuanzx.com

TS:   /error/gim
来源：http://cin.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xfz.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fcr.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://vig.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kkd.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://qbr.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imt.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pzk.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffj.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ukv.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://twi.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nmn.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qht.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iwa.yvedp.cn

================================================================================
来源：http://vxj.fzhhl.top

J. 日期与时间
来源：http://vyo.vqdsnc.cn

================================================================================
来源：http://aqq.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://qvh.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gpi.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://opv.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://ukz.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://myk.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://inw.jinqigfzy.top

Go:   time.Now()
来源：http://lyo.meibo888.top

Ruby: Time.now
来源：http://nqm.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bqm.redwolf501.top

[J02] 格式化输出
来源：http://cjd.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlx.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lhf.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rzz.wangshuangyany.cn

TS:   d.toISOString()
来源：http://exo.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zgh.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fcy.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ouy.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vkb.bjfxy.top


<!-- 参考信息 -->