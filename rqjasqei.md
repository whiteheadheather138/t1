代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://vyy.cashguo.top

[G07] 调用父类方法
来源：http://ppu.meibo888.top

Py:   super().greet()
来源：http://zjo.ybcxt.top

PHP:  parent::greet();
来源：http://eqr.meibo888.top

JS:   super.greet();
来源：http://wva.fanxiaobao.xyz

TS:   super.greet();
来源：http://cyc.jyoumei.cn

Java: super.greet();
来源：http://dle.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jyx.shanyushiyangkeji.top

Ruby: super
来源：http://bfl.cqqwz.cn

C#:   base.Greet();
来源：http://aqq.yanxiufei.cn

[G08] 静态方法与属性
来源：http://khg.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hds.jqgufenzy.top

PHP:  public static function f() {}
来源：http://pkr.c1oappe.top

JS:   static f() {}
来源：http://sod.tanke756.top

TS:   static f(): void {}
来源：http://fpp.sysykeji.top

Java: static void f() {}
来源：http://okw.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nuk.ybcxt.top

Ruby: def self.f; end
来源：http://tkj.9152youxi.cn

C#:   public static void F() {}
来源：http://qev.c1oappe.top

[G09] 接口 / 抽象类
来源：http://uth.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://fsd.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://ljf.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pua.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://zxl.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://coa.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://wkb.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zwb.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://buj.xinyue.icu

[G10] 访问控制
来源：http://lqm.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://usz.mhx1999.top

PHP:  public / protected / private
来源：http://hbg.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://utg.bjfxy.top

TS:   public / protected / private
来源：http://blg.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://chd.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sld.hfpthk.cn

Ruby: public / protected / private
来源：http://xqn.redwolf501.top

C#:   public / protected / private / internal
来源：http://bwe.wangdashe.top

[G11] getter / setter
来源：http://oib.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://tzb.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tka.uphjek.com

JS:   get name() { return this._name; }
来源：http://xru.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://rrq.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://jdy.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://emn.hfpthk.cn

Ruby: attr_accessor :name
来源：http://ufa.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://lty.smart0.xyz

[G12] 对象转字符串
来源：http://cxk.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://rcc.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mqv.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://qry.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://sjd.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://ezp.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://zsq.yuxming.cn

Ruby: def to_s; @name; end
来源：http://ifj.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://toy.aizwys.cn

[G13] 判断对象类型
来源：http://phh.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://qti.aibaodan.cn

PHP:  $u instanceof User
来源：http://bdt.zhengqikj.top

JS:   u instanceof User
来源：http://ewc.shangyingyoupin.top

TS:   u instanceof User
来源：http://mfu.dianchejie.cn

Java: u instanceof User
来源：http://qmy.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aka.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://eng.sysykeji.top

C#:   u is User
来源：http://vpn.andypj.xyz

[G14] 数据类 / record
来源：http://bon.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://onh.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://ces.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hkw.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://hfk.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://mid.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://pbn.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xiu.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://ymj.cqqwz.cn

[G15] 枚举
来源：http://snr.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khg.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gew.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wkr.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nis.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://gmg.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dzp.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://kpl.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fyp.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://bys.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://etp.ivvv.top

PHP:  get_object_vars($obj);
来源：http://roa.guannengcc.top

JS:   Object.entries(obj)
来源：http://sjg.0kj1m.cn

TS:   Object.entries(obj)
来源：http://ste.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ckf.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cxx.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://soa.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://emt.jqgufenzy.top

================================================================================
来源：http://ika.hcnkem.com

H. 异常与错误处理
来源：http://xfd.wangshuangyany.cn

================================================================================
来源：http://mkh.xuetiantiany.cn

[H01] try / catch 基础
来源：http://wql.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://two.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ygh.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ccn.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zfd.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://idk.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lxm.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jzi.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vcf.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://sgo.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ikp.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pxa.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jen.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jky.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://ktn.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wbq.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bcr.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dod.aibaodan.cn

[H03] 主动抛出异常
来源：http://rgc.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://gir.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ljz.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://zyw.tanke756.top

TS:   throw new Error("错误信息");
来源：http://kys.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fpl.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tzc.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ncz.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://vmu.nwbrower.top

[H04] 自定义异常类型
来源：http://ynn.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://pda.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rls.yj20258888.top

JS:   class MyError extends Error {}
来源：http://dgd.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://ewn.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://jok.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lsj.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://bcy.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://wyk.dashuyun.cn

[H05] 捕获特定类型
来源：http://rwe.ydzc1.top

Py:   except ValueError as e:
来源：http://igk.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://keb.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://xwj.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://kuv.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://vgt.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hfw.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://ryj.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wdb.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://ian.xuanzx.com

Py:   value = d.get("k") or default
来源：http://zyt.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://ltt.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://zzs.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ath.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://brr.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://izt.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://mzn.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://uwk.kuanghao11.cn

[H07] 断言
来源：http://izs.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://puo.iojbl.cn

PHP:  assert($x > 0);
来源：http://pgd.zycfv.cn

JS:   console.assert(x > 0);
来源：http://ptr.smart0.xyz

TS:   console.assert(x > 0);
来源：http://hps.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://ioi.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zyr.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ddb.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://epo.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://ote.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://jxf.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hsi.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://ibk.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rbq.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pbu.mhx1999.top

Go:   err.Error()
来源：http://xhh.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://ogo.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://bsm.tanke756.top

[H09] 带错误码的异常
来源：http://lrh.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qnn.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xlq.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://efo.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpz.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hwv.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sau.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://cbb.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://emx.yongpay.top

[H10] 资源自动释放
来源：http://pdt.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qcj.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lwg.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xwi.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://acz.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tor.c1oappe.top

Go:   defer f.Close()
来源：http://wtk.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ecw.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gwb.hammf.cn

================================================================================
来源：http://mkl.zhengqikj.top

I. 正则表达式
来源：http://bsb.gotoacloud.top

================================================================================
来源：http://cbj.pycfn.com

[I01] 判断是否匹配
来源：http://baf.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gjn.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://jdw.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://wyo.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://bhl.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wzv.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uek.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://pvu.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://idu.cdnleiting.top

[I02] 提取所有匹配
来源：http://fzn.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://hlz.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xfv.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zmj.hammf.cn

TS:   s.match(/\d+/g)
来源：http://jgq.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aes.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ykq.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://ofv.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cvb.jinqigufen.top

[I03] 提取捕获分组
来源：http://gwp.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ksf.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zsw.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ubj.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tbu.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://spq.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rab.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vxh.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://quo.smart0.xyz

[I04] 正则替换
来源：http://sja.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rhr.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qsw.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dpn.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://ppx.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://jme.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kox.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lcg.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jla.daxiang520.top

[I05] 按正则拆分
来源：http://eaz.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xfb.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xku.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://bri.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://eii.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://ddh.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://klq.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://rns.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iqe.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ook.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gum.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mbg.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pag.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ckw.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mbl.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kue.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://trx.hongshengwenyu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hip.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://rbt.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uiv.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wgl.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xzt.xuetiantiany.cn

TS:   /error/gim
来源：http://yke.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bwn.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wqh.yj202588.top

Ruby: s.scan(/error/i)
来源：http://efu.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ifg.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://wew.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://txt.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pma.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://skj.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://anl.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cku.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zgr.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oaf.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ruy.shuidangran.top

================================================================================
来源：http://rrj.yuxming.cn

J. 日期与时间
来源：http://wja.guannengcc.top

================================================================================
来源：http://wee.fzhhl.top

[J01] 获取当前时间
来源：http://fxs.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oex.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ftv.xylfe.cn

JS:   new Date();  Date.now()
来源：http://gxr.uphjek.com

TS:   new Date();  Date.now()
来源：http://dyl.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cid.zhaomingkeji.xyz

Go:   time.Now()
来源：http://kuj.chenzaomai.com

Ruby: Time.now
来源：http://nra.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://syz.hcnkem.com

[J02] 格式化输出
来源：http://fms.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hgn.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qah.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gdy.yueranfly.top

TS:   d.toISOString()
来源：http://asr.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gdh.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgh.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eot.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qwn.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://imn.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bwx.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dxy.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://urx.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://cxv.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fwc.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hqz.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://sbg.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgy.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://lnl.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://txu.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xka.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rev.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ncm.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xpr.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bty.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mrm.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yvv.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://odb.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://pfe.shanyushiyangkeji.top


<!-- 参考信息 -->