代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://gnb.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://zcv.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://ius.yuxming.cn

Java: String greet() { return name; }
来源：http://xko.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wis.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://pgf.gzhubu.top

C#:   public string Greet() => Name;
来源：http://ccz.jinghuilouyu.cn

[G05] 继承
来源：http://iwa.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://uqz.daxiang520.top

PHP:  class Admin extends User {}
来源：http://ygg.yueranfly.top

JS:   class Admin extends User {}
来源：http://ejf.smart0.xyz

TS:   class Admin extends User {}
来源：http://ski.yangfankeji.com

Java: class Admin extends User {}
来源：http://tgo.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pkm.hammf.cn

Ruby: class Admin < User; end
来源：http://cgp.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://ffh.jinqigfzy.top

[G06] 重写方法
来源：http://xyd.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://chr.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://scm.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://pnz.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://ncy.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://yte.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mdg.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://snl.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://ddb.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://npb.xylfe.cn

Py:   super().greet()
来源：http://btj.ydjk.org.cn

PHP:  parent::greet();
来源：http://rvf.gzhubu.top

JS:   super.greet();
来源：http://opq.jinyuanbaomall.cn

TS:   super.greet();
来源：http://dqj.sysykeji.top

Java: super.greet();
来源：http://kkh.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bdq.zhiwuduotai.top

Ruby: super
来源：http://kbr.hfpthk.cn

C#:   base.Greet();
来源：http://nrr.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://ypo.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nza.gaohongyu789.top

PHP:  public static function f() {}
来源：http://ixq.birdmap.top

JS:   static f() {}
来源：http://qvf.yvedp.cn

TS:   static f(): void {}
来源：http://ojw.yuanzhike.top

Java: static void f() {}
来源：http://qtg.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kea.iojbl.cn

Ruby: def self.f; end
来源：http://apt.tanke756.top

C#:   public static void F() {}
来源：http://jcc.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://ont.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://ztq.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://jdt.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ncp.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://zsa.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://jye.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://jfe.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bfq.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://igz.ivvv.top

[G10] 访问控制
来源：http://xcd.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ecc.gogol.net.cn

PHP:  public / protected / private
来源：http://unn.bjfxy.top

JS:   #private 字段；其余公开
来源：http://eks.zhongyouzk.top

TS:   public / protected / private
来源：http://obz.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://mtu.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eta.sufxvd.cn

Ruby: public / protected / private
来源：http://bai.daria6918.cn

C#:   public / protected / private / internal
来源：http://ipq.gotoacloud.top

[G11] getter / setter
来源：http://myf.aizwys.cn

Py:   @property 与 @x.setter
来源：http://vtq.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fbh.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://mwq.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://myk.ehwqpu.com

Java: public String getName() { return name; }
来源：http://stz.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vch.aizwys.cn

Ruby: attr_accessor :name
来源：http://hlh.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://cpo.yvedp.cn

[G12] 对象转字符串
来源：http://wig.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://chm.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://okw.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://xbk.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://did.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://sbq.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ove.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://cjr.pycfn.com

C#:   public override string ToString() => Name;
来源：http://xhp.aizwys.cn

[G13] 判断对象类型
来源：http://vid.pycfn.com

Py:   isinstance(u, User)
来源：http://oab.52xcode.cn

PHP:  $u instanceof User
来源：http://mab.uphjek.com

JS:   u instanceof User
来源：http://kkq.yvedp.cn

TS:   u instanceof User
来源：http://two.havefunace.top

Java: u instanceof User
来源：http://ulx.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tfu.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://wnw.yj20258888.top

C#:   u is User
来源：http://jvi.zhijiandao.cn

[G14] 数据类 / record
来源：http://ahg.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fiv.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ybc.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://hqb.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://env.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://ezk.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://yab.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cji.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://xch.guannengcc.top

[G15] 枚举
来源：http://upi.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jqm.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsi.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jhr.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fgn.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://yse.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cqu.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://afy.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aze.ivvv.top

[G16] 对象转数组 / 字典
来源：http://sdf.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uex.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://bwv.yongpay.top

JS:   Object.entries(obj)
来源：http://muo.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://nrb.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://grm.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gpu.0kj1m.cn

Ruby: obj.instance_variables
来源：http://mwv.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://prm.zhixingplan.top

================================================================================
来源：http://ppe.jqgfzy.top

H. 异常与错误处理
来源：http://aor.hywenlv.cn

================================================================================
来源：http://lwx.fktsv.cn

[H01] try / catch 基础
来源：http://nwz.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ykb.ehwqpu.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nni.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gwi.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ngl.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ual.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hin.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://orz.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://auv.andypj.xyz

[H02] finally / ensure 收尾
来源：http://nbw.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://raw.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rbk.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://eib.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wdf.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vve.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lug.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jiu.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nao.zhijiandao.cn

[H03] 主动抛出异常
来源：http://zoc.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://bpq.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hvm.316326.xyz

JS:   throw new Error("错误信息");
来源：http://xyn.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://kuh.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yhg.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fpb.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lzx.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://dvl.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://cbb.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://wup.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ozo.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://dqs.0kj1m.cn

TS:   class MyError extends Error {}
来源：http://zvr.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://ubz.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nru.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://ncn.fzhhl.top

C#:   class MyException : Exception {}
来源：http://nvx.jqgfzy.top

[H05] 捕获特定类型
来源：http://kbs.pycfn.com

Py:   except ValueError as e:
来源：http://xje.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mzm.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://hcu.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://tiq.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://mnu.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gpx.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://gel.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wwy.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://bes.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://smg.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ivx.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://xxl.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://gbt.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qpc.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zke.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://ouy.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://xhm.yongpay.top

[H07] 断言
来源：http://xbj.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://bab.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://fco.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://fys.hesvh.cn

TS:   console.assert(x > 0);
来源：http://bpe.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://zse.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jkg.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://tha.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://bcu.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://eiq.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://anl.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ald.wangdashe.top

JS:   e.message;  e.stack
来源：http://gqa.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rte.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jen.c1oappe.top

Go:   err.Error()
来源：http://qbu.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://wba.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://wbz.ydjk.org.cn

[H09] 带错误码的异常
来源：http://uki.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://urm.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ghw.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://boh.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ffb.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ptd.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gzj.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kpa.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://woc.yueranfly.top

[H10] 资源自动释放
来源：http://fdp.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vxj.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lxz.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qwv.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xmp.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wvx.yj202588.top

Go:   defer f.Close()
来源：http://ham.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xro.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wmd.gzhubu.top

================================================================================
来源：http://krl.hywenlv.cn

I. 正则表达式
来源：http://utg.ydzc1.top

================================================================================
来源：http://ydu.316326.xyz

[I01] 判断是否匹配
来源：http://mco.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dum.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://lkq.mhx1999.top

JS:   /\d+/.test(s)
来源：http://deb.yonumen.top

TS:   /\d+/.test(s)
来源：http://pjo.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://whm.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kze.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://fan.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jgx.jinqigufen.top

[I02] 提取所有匹配
来源：http://tuc.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://ejz.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mob.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gmb.havefunace.top

TS:   s.match(/\d+/g)
来源：http://ssq.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uar.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xmv.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://gvj.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://siz.iojbl.cn

[I03] 提取捕获分组
来源：http://jdn.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cpp.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iuz.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aev.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cgy.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mzm.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hxv.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://snf.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sud.9152youxi.cn

[I04] 正则替换
来源：http://zct.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zyy.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kqs.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://mak.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://lmq.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://aki.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fkx.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://snb.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dbx.yanxiufei.cn

[I05] 按正则拆分
来源：http://dpq.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://emb.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gyv.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://fkw.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://buz.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://gbm.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xij.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yxk.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yjz.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hmj.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eiz.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rct.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkq.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bon.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hxv.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://voj.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://khl.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eqm.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://rsz.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mpo.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bmi.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://itl.andypj.xyz

TS:   /error/gim
来源：http://axo.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uvb.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rsl.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://zep.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://phj.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://qwu.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yrz.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbf.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bvg.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fag.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ptc.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bfm.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wmh.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sfa.fehbvm.com

================================================================================
来源：http://qqx.ydjk.org.cn

J. 日期与时间
来源：http://mgw.mhx1999.top

================================================================================
来源：http://wvv.shangyingyoupin.top

[J01] 获取当前时间
来源：http://yxd.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hmq.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wah.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://gae.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://xxj.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://yfs.gzhubu.top

Go:   time.Now()
来源：http://zpl.nanxuanxn.top

Ruby: Time.now
来源：http://klj.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lpd.chenjidiqi.icu

[J02] 格式化输出
来源：http://hsn.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekh.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kpx.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wmh.cqqwz.cn

TS:   d.toISOString()
来源：http://jgo.zdqjudy.top


<!-- 参考信息 -->