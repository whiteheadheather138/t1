代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://vur.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://yvl.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jhq.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://xdf.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://ewg.cashguo.top

[G07] 调用父类方法
来源：http://lav.ydjk.org.cn

Py:   super().greet()
来源：http://cas.ehwqpu.com

PHP:  parent::greet();
来源：http://pez.zycfv.cn

JS:   super.greet();
来源：http://jcc.jqgufenzy.top

TS:   super.greet();
来源：http://hcy.yueranfly.top

Java: super.greet();
来源：http://awn.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sjq.hnxiangtu.top

Ruby: super
来源：http://vsi.ybcxt.top

C#:   base.Greet();
来源：http://efa.fehbvm.com

[G08] 静态方法与属性
来源：http://cky.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tnc.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://ums.yonumen.top

JS:   static f() {}
来源：http://smy.tanke756.top

TS:   static f(): void {}
来源：http://ysg.shzxlz.cn

Java: static void f() {}
来源：http://uen.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tgg.wangshuangyany.cn

Ruby: def self.f; end
来源：http://pue.shzxlz.cn

C#:   public static void F() {}
来源：http://umc.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://cgu.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://ncw.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pcz.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://orl.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://tvy.zycfv.cn

Java: interface Shape { double area(); }
来源：http://rnu.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://aex.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://orf.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://usn.iojbl.cn

[G10] 访问控制
来源：http://izx.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ezq.epnwcf.com

PHP:  public / protected / private
来源：http://fzi.xinyue.icu

JS:   #private 字段；其余公开
来源：http://fqe.nwbrower.top

TS:   public / protected / private
来源：http://ilm.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://xhr.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gjk.yangfankeji.com

Ruby: public / protected / private
来源：http://xdk.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://ama.52xcode.cn

[G11] getter / setter
来源：http://cyl.ybcxt.top

Py:   @property 与 @x.setter
来源：http://ocd.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://qxj.meibo888.top

JS:   get name() { return this._name; }
来源：http://eep.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://ihv.xylfe.cn

Java: public String getName() { return name; }
来源：http://lem.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xhf.snrcjt.cn

Ruby: attr_accessor :name
来源：http://jop.fehbvm.com

C#:   public string Name { get; set; }
来源：http://wxr.316326.xyz

[G12] 对象转字符串
来源：http://lsy.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://hyq.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://akb.hesvh.cn

JS:   toString() { return this.name; }
来源：http://rdl.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://zdv.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://pis.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://wrl.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://yru.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://pnq.yj202588.top

[G13] 判断对象类型
来源：http://rdt.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://okq.tian-w.cn

PHP:  $u instanceof User
来源：http://zwb.fehbvm.com

JS:   u instanceof User
来源：http://hio.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://jib.chenzaomai.com

Java: u instanceof User
来源：http://xrg.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ctw.yongpay.top

Ruby: u.is_a?(User)
来源：http://fgt.yueranfly.top

C#:   u is User
来源：http://uso.0kj1m.cn

[G14] 数据类 / record
来源：http://aiw.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cye.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://otd.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://yrg.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://cmq.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://yjr.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://zom.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lvk.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://wzl.nanxinkj.top

[G15] 枚举
来源：http://lit.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jaf.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ees.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqq.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mvq.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://wrl.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://goe.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://rgr.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://geq.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://fuc.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rmx.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://gte.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://iry.aibaodan.cn

TS:   Object.entries(obj)
来源：http://gfm.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oiy.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uef.iojbl.cn

Ruby: obj.instance_variables
来源：http://rlt.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://zvv.shanyushiyangkeji.top

================================================================================
来源：http://kfu.ivvv.top

H. 异常与错误处理
来源：http://nes.jianghu66.top

================================================================================
来源：http://asx.vehdjk.com

[H01] try / catch 基础
来源：http://qww.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gfe.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ymk.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xin.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mjg.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mdr.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://thb.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hyq.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uks.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://gpn.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tay.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fca.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ste.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://hxy.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://xtx.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://srz.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hqk.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hak.sysykeji.top

[H03] 主动抛出异常
来源：http://nuk.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://qui.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nzs.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://zob.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://xpx.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lyw.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pjv.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lbn.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://nbx.bjfxy.top

[H04] 自定义异常类型
来源：http://ybl.birdmap.top

Py:   class MyError(Exception): pass
来源：http://pxq.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://mco.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://lzl.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://ebk.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://kyn.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wtq.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://xow.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://cuc.smart0.xyz

[H05] 捕获特定类型
来源：http://ccm.mhx1999.top

Py:   except ValueError as e:
来源：http://bmy.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uun.daxiang520.top

JS:   if (e instanceof TypeError) {}
来源：http://wcc.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://rli.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://sos.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dsh.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://qhf.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pig.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://gdj.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://emm.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://erd.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://slt.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://pap.yueranfly.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mwx.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://npc.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://zwt.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://xrr.xziqi.cn

[H07] 断言
来源：http://cud.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://qcd.fehbvm.com

PHP:  assert($x > 0);
来源：http://xib.yonumen.top

JS:   console.assert(x > 0);
来源：http://wcu.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://cnd.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://ewe.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwl.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://npe.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://yoz.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://omp.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://vlb.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ssh.chenzaomai.com

JS:   e.message;  e.stack
来源：http://drp.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xsq.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ijo.nwbrower.top

Go:   err.Error()
来源：http://ldb.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://sml.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://sur.sweek.top

[H09] 带错误码的异常
来源：http://amb.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tul.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wjr.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://swk.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vbs.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pkv.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nwk.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://azq.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yur.kuanghao11.cn

[H10] 资源自动释放
来源：http://esh.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://nqc.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uyy.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://quq.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zqk.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kun.zhengqikj.top

Go:   defer f.Close()
来源：http://bmy.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zys.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nxl.gzhubu.top

================================================================================
来源：http://vdz.yj20258888.top

I. 正则表达式
来源：http://cpo.havefunace.top

================================================================================
来源：http://qri.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://mez.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pda.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://tkl.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://ggz.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://rpi.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rge.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ryz.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://uhn.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cib.gaohongyu789.top

[I02] 提取所有匹配
来源：http://fyr.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://jgq.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bkz.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zsb.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://szh.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hpn.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mwc.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://alz.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rxr.cucudq.cn

[I03] 提取捕获分组
来源：http://jrk.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dcu.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wua.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gii.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kwv.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mpj.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xcr.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lyw.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qsr.xylfe.cn

[I04] 正则替换
来源：http://cmm.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yxg.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uiy.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://ttl.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://lgv.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://dxl.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gmq.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uoh.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://slz.zhengqikj.top

[I05] 按正则拆分
来源：http://tru.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iwt.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rlr.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://bay.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://vdk.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://qjr.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ime.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uod.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://itz.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ezf.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sst.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wux.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkx.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bdl.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qvp.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://led.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sad.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gka.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://fty.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rjn.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://azb.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hop.feifeiyinyue.top

TS:   /error/gim
来源：http://lhl.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mxi.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://saw.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://sxe.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hxf.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://ebp.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ron.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://snm.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqv.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofl.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zlp.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nxx.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpb.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lwd.zhoulong.xyz

================================================================================
来源：http://vyd.shangyingyoupin.top

J. 日期与时间
来源：http://bgf.zycfv.cn

================================================================================
来源：http://tjt.epnwcf.com

[J01] 获取当前时间
来源：http://hnl.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gmc.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jqy.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://mzl.gzhubu.top

TS:   new Date();  Date.now()
来源：http://qow.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cui.zhengqikj.top

Go:   time.Now()
来源：http://lgr.hongshengwenyu.top

Ruby: Time.now
来源：http://xzj.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lej.fzhhl.top

[J02] 格式化输出
来源：http://znu.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cgk.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rsx.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bft.jyoumei.cn

TS:   d.toISOString()
来源：http://wsg.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dsd.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zwz.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bkp.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://buq.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://fdg.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wlf.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pjx.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://exp.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://yin.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://gmg.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uia.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://hca.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vnk.guannengcc.top

[J04] 时间戳与日期互转
来源：http://wae.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ete.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vbr.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zns.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wrp.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nml.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qaf.snrcjt.cn


<!-- 参考信息 -->