代发 wailian999

Java: class Admin extends User {}
来源：http://qar.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nny.zhixingplan.top

Ruby: class Admin < User; end
来源：http://lhy.yangfankeji.com

C#:   class Admin : User {}
来源：http://por.xuetiantiany.cn

[G06] 重写方法
来源：http://nht.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://sqa.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://atu.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://mac.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://vdr.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jwi.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tsh.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://fmj.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://tze.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://phv.fehbvm.com

Py:   super().greet()
来源：http://zoq.nanxuanxn.top

PHP:  parent::greet();
来源：http://vdo.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://ltp.52xcode.cn

TS:   super.greet();
来源：http://hid.pengpengdd.cyou

Java: super.greet();
来源：http://luw.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cha.fengsongda.top

Ruby: super
来源：http://sjd.chenlongwang.top

C#:   base.Greet();
来源：http://hme.jqgufenzy.top

[G08] 静态方法与属性
来源：http://dgx.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nvn.shzxlz.cn

PHP:  public static function f() {}
来源：http://nlm.sweek.top

JS:   static f() {}
来源：http://aui.hesvh.cn

TS:   static f(): void {}
来源：http://ucb.guowangkeji.top

Java: static void f() {}
来源：http://vrc.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ltb.redwolf501.top

Ruby: def self.f; end
来源：http://yjf.yanxiufei.cn

C#:   public static void F() {}
来源：http://pzv.epnwcf.com

[G09] 接口 / 抽象类
来源：http://vez.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://was.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://zjp.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rau.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://zav.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://czq.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ubs.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ysh.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://naz.iojbl.cn

[G10] 访问控制
来源：http://fjs.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://eam.svipenyu.cn

PHP:  public / protected / private
来源：http://qhh.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://rlq.smart0.xyz

TS:   public / protected / private
来源：http://fzr.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://xqu.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rls.xuetiantiany.cn

Ruby: public / protected / private
来源：http://gef.ivvv.top

C#:   public / protected / private / internal
来源：http://jue.guowangkeji.top

[G11] getter / setter
来源：http://bzs.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://paq.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oey.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://xly.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://lbf.zdbjq.cn

Java: public String getName() { return name; }
来源：http://bai.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tgo.0kj1m.cn

Ruby: attr_accessor :name
来源：http://gtq.xziqi.cn

C#:   public string Name { get; set; }
来源：http://gdt.cdnleiting.top

[G12] 对象转字符串
来源：http://ltx.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://qrr.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kah.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://qbg.gaohongyu789.top

TS:   toString(): string { return this.name; }
来源：http://xig.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://aoi.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://bqr.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://nqx.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://ues.feifeiyinyue.top

[G13] 判断对象类型
来源：http://lnn.yvedp.cn

Py:   isinstance(u, User)
来源：http://xyi.zhixingplan.top

PHP:  $u instanceof User
来源：http://ace.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://huk.yvedp.cn

TS:   u instanceof User
来源：http://xqz.yonumen.top

Java: u instanceof User
来源：http://wxt.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jvy.epnwcf.com

Ruby: u.is_a?(User)
来源：http://wue.yongpay.top

C#:   u is User
来源：http://rhr.ctjpmb.com

[G14] 数据类 / record
来源：http://dye.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tst.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://yvk.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://tvu.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://jcs.bjfxy.top

Java: record User(String name, int age) {}
来源：http://hzo.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://hfm.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nfa.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://wsb.zhixingplan.top

[G15] 枚举
来源：http://ean.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eut.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://onp.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mtu.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://omo.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://ixe.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ohn.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://fgq.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://umz.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://xrq.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://isk.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://emn.yvedp.cn

JS:   Object.entries(obj)
来源：http://xbv.pycfn.com

TS:   Object.entries(obj)
来源：http://umc.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ebk.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kcp.pycfn.com

Ruby: obj.instance_variables
来源：http://ovy.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://lzs.ehwqpu.com

================================================================================
来源：http://ewy.zhengqikj.top

H. 异常与错误处理
来源：http://zao.ywan-chungtsiang.top

================================================================================
来源：http://ban.chenlongwang.top

[H01] try / catch 基础
来源：http://sru.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cgf.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mze.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://evq.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gph.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://czu.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iim.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zih.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vsr.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://yqe.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://khz.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eeu.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lrz.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kda.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://tnl.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ktr.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://suq.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hxk.aibaodan.cn

[H03] 主动抛出异常
来源：http://vnq.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://xee.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vyd.ivvv.top

JS:   throw new Error("错误信息");
来源：http://xah.ivvv.top

TS:   throw new Error("错误信息");
来源：http://fxa.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qrv.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xdf.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://zyk.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://len.0kj1m.cn

[H04] 自定义异常类型
来源：http://iru.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://nvq.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://mwl.xinyue.icu

JS:   class MyError extends Error {}
来源：http://hnc.andypj.xyz

TS:   class MyError extends Error {}
来源：http://phc.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://lme.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sgy.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://nsh.cashguo.top

C#:   class MyException : Exception {}
来源：http://wym.tarul.cn

[H05] 捕获特定类型
来源：http://vrp.bbcook.cn

Py:   except ValueError as e:
来源：http://cji.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ule.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://mmb.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://jdx.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://nqw.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tse.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://pbr.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zyz.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://cpp.redwolf501.top

Py:   value = d.get("k") or default
来源：http://icb.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://ibg.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ort.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dop.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rjj.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://joz.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://wfw.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://klz.jinghuilouyu.cn

[H07] 断言
来源：http://und.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://mcv.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://uqm.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://oyu.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://gux.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://ews.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cjd.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://etf.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://nye.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://skz.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://cat.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dmv.ctjpmb.com

JS:   e.message;  e.stack
来源：http://jqq.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwi.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rrk.aizwys.cn

Go:   err.Error()
来源：http://bec.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://vrj.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://vwm.zhixingplan.top

[H09] 带错误码的异常
来源：http://urw.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jea.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uuq.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xvg.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://swb.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fum.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fcb.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zbz.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://pkk.jqgfzy.top

[H10] 资源自动释放
来源：http://hkb.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dja.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cbh.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eac.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://plu.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zmg.iojbl.cn

Go:   defer f.Close()
来源：http://rov.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ape.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gig.mhx1999.top

================================================================================
来源：http://upu.cqqwz.cn

I. 正则表达式
来源：http://rqb.guowangkeji.top

================================================================================
来源：http://zxr.sysykeji.top

[I01] 判断是否匹配
来源：http://kum.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oek.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://btf.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://gvp.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://skr.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xqe.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yha.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://jsd.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vga.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://lmf.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://ahe.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oix.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kok.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://wpo.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pub.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dur.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://eik.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zyp.ybcxt.top

[I03] 提取捕获分组
来源：http://pcm.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nxq.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://guf.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uxb.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ezw.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ewh.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rlr.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kqn.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cwj.ywan-chungtsiang.top

[I04] 正则替换
来源：http://ber.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zcg.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ewa.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://zka.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://itu.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://xwm.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yic.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jim.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ady.yongpay.top

[I05] 按正则拆分
来源：http://neg.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hhw.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uif.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://xfy.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://ata.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://cvn.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oek.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://yzu.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tna.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dve.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fin.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pzr.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zpe.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sae.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vny.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://age.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixv.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xws.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://rsd.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cue.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pxu.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ksw.daxiang520.top

TS:   /error/gim
来源：http://pvj.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ofu.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mwp.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://ctn.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://otm.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ylw.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sra.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://riz.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hyy.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qrk.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qkl.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vlz.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lxk.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fnr.zhongyouzk.top

================================================================================
来源：http://chj.sysykeji.top

J. 日期与时间
来源：http://yww.shanyushiyangtech.top

================================================================================
来源：http://fvk.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://lso.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://hrz.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gzo.yj20258888.top

JS:   new Date();  Date.now()
来源：http://ytq.sweek.top

TS:   new Date();  Date.now()
来源：http://qbk.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yra.tarul.cn

Go:   time.Now()
来源：http://jlq.feifeiyinyue.top

Ruby: Time.now
来源：http://uyo.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sss.sjlbkw.cn

[J02] 格式化输出
来源：http://voc.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vul.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xxh.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dpq.snrcjt.cn

TS:   d.toISOString()
来源：http://kug.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jes.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hzi.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eqy.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://odf.xinyue.icu

[J03] 字符串解析为日期
来源：http://zla.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xzt.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yti.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://yac.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://pqh.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://tff.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sqr.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://cyr.zhiwuduotai.top


<!-- 参考信息 -->