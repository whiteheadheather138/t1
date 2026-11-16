代发 wailian999

Py:   class Admin(User): pass
来源：http://qwd.aizwys.cn

PHP:  class Admin extends User {}
来源：http://gof.yj20258.top

JS:   class Admin extends User {}
来源：http://zgb.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://brn.cqqwz.cn

Java: class Admin extends User {}
来源：http://myw.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rjc.uphjek.com

Ruby: class Admin < User; end
来源：http://tta.shuidangran.top

C#:   class Admin : User {}
来源：http://hcr.uphjek.com

[G06] 重写方法
来源：http://oyv.pycfn.com

Py:   def greet(self): return "admin"
来源：http://usx.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nbx.tarul.cn

JS:   greet() { return "admin"; }
来源：http://jhk.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://apq.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://zuk.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://myj.tarul.cn

Ruby: def greet; "admin"; end
来源：http://ezm.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://qll.vqdsnc.cn

[G07] 调用父类方法
来源：http://vgz.dianchejie.cn

Py:   super().greet()
来源：http://eoj.gzhubu.top

PHP:  parent::greet();
来源：http://jgu.yvedp.cn

JS:   super.greet();
来源：http://ork.zhaomingkeji.xyz

TS:   super.greet();
来源：http://jry.gogol.net.cn

Java: super.greet();
来源：http://mxx.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ccd.jiagoushi.top

Ruby: super
来源：http://yys.shanyushiyangtech.top

C#:   base.Greet();
来源：http://nts.ctjpmb.com

[G08] 静态方法与属性
来源：http://kgf.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbd.yuxming.cn

PHP:  public static function f() {}
来源：http://myj.zhongyouzk.top

JS:   static f() {}
来源：http://dqq.wangdashe.top

TS:   static f(): void {}
来源：http://hmu.dashuyun.cn

Java: static void f() {}
来源：http://mgg.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://plv.guowangkeji.top

Ruby: def self.f; end
来源：http://bqj.dianchejie.cn

C#:   public static void F() {}
来源：http://wxp.vehdjk.com

[G09] 接口 / 抽象类
来源：http://ulh.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://jhb.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://ayf.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://muh.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://xcd.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://hxb.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://wld.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://myd.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://ahv.xziqi.cn

[G10] 访问控制
来源：http://vst.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://jqp.smart0.xyz

PHP:  public / protected / private
来源：http://gqd.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://ypv.hcnkem.com

TS:   public / protected / private
来源：http://pip.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://nmr.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kgr.jqgfzy.top

Ruby: public / protected / private
来源：http://ssz.yueranfly.top

C#:   public / protected / private / internal
来源：http://bzl.bjfxy.top

[G11] getter / setter
来源：http://oow.tarul.cn

Py:   @property 与 @x.setter
来源：http://ild.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bag.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://bws.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://wyd.dashuyun.cn

Java: public String getName() { return name; }
来源：http://jmh.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yvt.ivvv.top

Ruby: attr_accessor :name
来源：http://lhk.tanke756.top

C#:   public string Name { get; set; }
来源：http://hke.shuidangran.top

[G12] 对象转字符串
来源：http://ija.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://vpo.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tpq.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://oyk.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://dmp.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://jeg.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://bow.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://hkx.hammf.cn

C#:   public override string ToString() => Name;
来源：http://urd.zhiwuduotai.top

[G13] 判断对象类型
来源：http://vqz.yj20258888.top

Py:   isinstance(u, User)
来源：http://tlb.mhx1999.top

PHP:  $u instanceof User
来源：http://pkm.yonumen.top

JS:   u instanceof User
来源：http://nwf.vehdjk.com

TS:   u instanceof User
来源：http://pyo.shanyushiyangkeji.top

Java: u instanceof User
来源：http://eig.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nxm.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://hps.yj20258888.top

C#:   u is User
来源：http://sge.gogol.net.cn

[G14] 数据类 / record
来源：http://tio.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://egh.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://ury.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://puf.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://ylb.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://wms.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://xoe.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cbk.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://ogt.shangyingyoupin.top

[G15] 枚举
来源：http://ngc.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uec.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyy.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ilz.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jtj.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://ted.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://waa.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://xzc.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bjn.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://lqt.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jjf.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://wqo.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://ysc.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://ttf.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mtv.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gez.chenlongwang.top

Ruby: obj.instance_variables
来源：http://dmi.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://asr.shanyushiyangkeji.top

================================================================================
来源：http://ovh.dianchejie.cn

H. 异常与错误处理
来源：http://gox.xziqi.cn

================================================================================
来源：http://ikv.yvedp.cn

[H01] try / catch 基础
来源：http://eot.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kob.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vvf.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pcx.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://szd.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jxd.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lmt.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://twl.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xaf.andypj.xyz

[H02] finally / ensure 收尾
来源：http://cau.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wtj.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wbi.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qfa.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wht.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://unb.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kuf.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zpw.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ske.havefunace.top

[H03] 主动抛出异常
来源：http://tox.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://zvs.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pfh.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://nbw.yongpay.top

TS:   throw new Error("错误信息");
来源：http://mpd.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://biq.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nsj.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dll.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://jla.hnqzz.top

[H04] 自定义异常类型
来源：http://gbf.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://cyq.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uum.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://muk.gzhubu.top

TS:   class MyError extends Error {}
来源：http://acp.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://qbb.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dyr.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://abt.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://hzf.ivvv.top

[H05] 捕获特定类型
来源：http://wtk.tarul.cn

Py:   except ValueError as e:
来源：http://rqm.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://seu.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://jzd.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://gsf.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://xow.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://igf.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://suc.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xzl.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://vmz.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://eie.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hxz.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nxl.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://ljw.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pdw.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ijm.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://jed.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://lfq.aibaodan.cn

[H07] 断言
来源：http://sys.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://yqc.pycfn.com

PHP:  assert($x > 0);
来源：http://arr.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://okr.tian-w.cn

TS:   console.assert(x > 0);
来源：http://luh.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://cwb.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wnx.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://aeg.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://txa.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://bva.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://hmb.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mql.52xcode.cn

JS:   e.message;  e.stack
来源：http://ezi.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iun.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yck.birdmap.top

Go:   err.Error()
来源：http://nps.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://laz.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://rdy.dashuyun.cn

[H09] 带错误码的异常
来源：http://sak.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hsc.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jwt.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uuq.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://icw.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oye.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zki.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://lum.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hpz.xziqi.cn

[H10] 资源自动释放
来源：http://xok.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qac.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rfb.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hqz.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bbq.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xpp.haohaochexian.top

Go:   defer f.Close()
来源：http://lzi.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://htj.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://opd.yanxiufei.cn

================================================================================
来源：http://qod.shzxlz.cn

I. 正则表达式
来源：http://byw.tarul.cn

================================================================================
来源：http://rns.316326.xyz

[I01] 判断是否匹配
来源：http://hxq.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gyx.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mlp.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://nyr.hnqzz.top

TS:   /\d+/.test(s)
来源：http://tid.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vfh.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://khf.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://exh.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://znf.yonumen.top

[I02] 提取所有匹配
来源：http://wal.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://qnf.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tio.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dlz.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://bnc.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zmk.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oef.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://dnj.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tze.c1oappe.top

[I03] 提取捕获分组
来源：http://vhc.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lrk.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vvg.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://soq.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cqp.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qtz.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://apr.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zvk.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sot.iojbl.cn

[I04] 正则替换
来源：http://ovg.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lpx.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lig.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ntk.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://olc.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fia.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vum.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ytl.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kgd.jqgfzy.top

[I05] 按正则拆分
来源：http://zcz.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ebv.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wag.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://vsv.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://ctj.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://xaj.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rhy.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://buc.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hef.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gfk.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cwy.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://thd.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oef.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kah.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://szq.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zxt.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yfh.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sws.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://gbs.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tuk.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ylt.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iic.tian-w.cn

TS:   /error/gim
来源：http://fxp.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cwd.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xqz.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://zkc.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iwo.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://dod.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pxd.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bhh.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hmw.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ucl.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://spz.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tev.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jnu.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pbj.nanxuanxn.top

================================================================================
来源：http://jrm.bbcook.cn

J. 日期与时间
来源：http://nta.sxryk.cn

================================================================================
来源：http://awk.shuidangran.top

[J01] 获取当前时间
来源：http://ddu.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yvd.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lmx.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://hny.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://auw.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://khq.fktsv.cn

Go:   time.Now()
来源：http://odd.zdqjudy.top

Ruby: Time.now
来源：http://oiz.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xfp.nwbrower.top

[J02] 格式化输出
来源：http://xol.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ech.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://txz.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://coc.mhx1999.top

TS:   d.toISOString()
来源：http://cev.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dep.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wxn.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pxa.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ezp.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://eif.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://btq.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pwa.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://npe.wangshuangyany.cn


<!-- 参考信息 -->