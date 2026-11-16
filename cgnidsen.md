代发 wailian999

JS:   super.greet();
来源：http://bfo.yangfankeji.com

TS:   super.greet();
来源：http://dxk.tanke756.top

Java: super.greet();
来源：http://zsa.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://phq.kuanghao11.cn

Ruby: super
来源：http://vwt.yuanzhike.top

C#:   base.Greet();
来源：http://iau.gaohongyu789.top

[G08] 静态方法与属性
来源：http://aau.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gyu.vehdjk.com

PHP:  public static function f() {}
来源：http://zkr.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://meq.nanxinkj.top

TS:   static f(): void {}
来源：http://nti.sjlbkw.cn

Java: static void f() {}
来源：http://bzr.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://jtr.hnqzz.top

Ruby: def self.f; end
来源：http://bqt.jqgufenzy.top

C#:   public static void F() {}
来源：http://rgb.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://trm.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://mso.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://ikg.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lpq.xuanzx.com

TS:   interface Shape { area(): number; }
来源：http://glv.cucudq.cn

Java: interface Shape { double area(); }
来源：http://tes.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://joz.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xjz.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://yhh.gogol.net.cn

[G10] 访问控制
来源：http://wlt.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://opp.gogol.net.cn

PHP:  public / protected / private
来源：http://cho.gzhubu.top

JS:   #private 字段；其余公开
来源：http://tpg.zhiwuduotai.top

TS:   public / protected / private
来源：http://zjp.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://ycz.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nis.ydzc1.top

Ruby: public / protected / private
来源：http://ubg.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://ctl.ctjpmb.com

[G11] getter / setter
来源：http://aaj.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://jyl.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hzk.fanxiaobao.xyz

JS:   get name() { return this._name; }
来源：http://rhp.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://woj.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://qjt.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://fxb.yvedp.cn

Ruby: attr_accessor :name
来源：http://hzn.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://swq.zhoulong.xyz

[G12] 对象转字符串
来源：http://rpx.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://edq.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://hze.pycfn.com

JS:   toString() { return this.name; }
来源：http://wsj.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://nvw.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://tqu.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://sav.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://mvk.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://zgc.feifeiyinyue.top

[G13] 判断对象类型
来源：http://jmo.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://ajj.birdmap.top

PHP:  $u instanceof User
来源：http://zhd.svipenyu.cn

JS:   u instanceof User
来源：http://dwe.bbcook.cn

TS:   u instanceof User
来源：http://jny.xinyue.icu

Java: u instanceof User
来源：http://dst.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zjd.yongpay.top

Ruby: u.is_a?(User)
来源：http://sfc.yongpay.top

C#:   u is User
来源：http://fai.nanxinkj.top

[G14] 数据类 / record
来源：http://lge.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kjf.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://acy.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zps.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://ilm.xuanzx.com

Java: record User(String name, int age) {}
来源：http://poo.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://qod.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://esc.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://ziu.9152youxi.cn

[G15] 枚举
来源：http://xbk.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fkl.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hyx.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ngq.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bww.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://meu.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yiz.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://bhn.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://til.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://pmx.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://akm.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://pgb.nanxinkj.top

JS:   Object.entries(obj)
来源：http://pwe.haohaochexian.top

TS:   Object.entries(obj)
来源：http://hdu.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rwd.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ckb.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://xws.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://tcq.ivvv.top

================================================================================
来源：http://yfs.9152youxi.cn

H. 异常与错误处理
来源：http://djc.yangfankeji.com

================================================================================
来源：http://rax.yj20258888.top

[H01] try / catch 基础
来源：http://unu.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mfk.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cnf.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://seo.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ixg.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rua.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qev.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sgq.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rww.cashguo.top

[H02] finally / ensure 收尾
来源：http://ieo.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://pjz.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yjd.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://knz.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rrl.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://etv.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://mgd.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cvc.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ztn.vehdjk.com

[H03] 主动抛出异常
来源：http://zxy.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://ppp.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sqa.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://ixg.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://crv.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pap.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vud.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rbk.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xsd.cqqwz.cn

[H04] 自定义异常类型
来源：http://ntn.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://tjk.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://lht.ydzc1.top

JS:   class MyError extends Error {}
来源：http://ikk.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://sfv.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://esb.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xyh.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://rdx.xylfe.cn

C#:   class MyException : Exception {}
来源：http://yim.gaohongyu789.top

[H05] 捕获特定类型
来源：http://npy.hcnkem.com

Py:   except ValueError as e:
来源：http://noe.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vqy.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://yce.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://uco.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://cow.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://egn.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://mke.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jlj.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://qtw.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://ujc.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://leo.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://nbv.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://sph.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jih.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://flx.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://gyy.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://vhr.pycfn.com

[H07] 断言
来源：http://gsy.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://oyp.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://lsp.hnqzz.top

JS:   console.assert(x > 0);
来源：http://lfm.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://vuq.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://zvl.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gwu.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://uaq.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://iuv.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://xpg.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://gjh.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bmw.sufxvd.cn

JS:   e.message;  e.stack
来源：http://csu.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://olg.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bcs.quarkkingdee.top

Go:   err.Error()
来源：http://sgr.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://lwz.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://xtb.ybcxt.top

[H09] 带错误码的异常
来源：http://zqf.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vhe.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oak.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rxz.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://usa.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wvm.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dez.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://lmy.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://oot.jqgfzy.top

[H10] 资源自动释放
来源：http://gla.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yek.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://deg.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jzx.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dzx.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nmw.yuxming.cn

Go:   defer f.Close()
来源：http://mwm.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qzi.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://klw.dianchejie.cn

================================================================================
来源：http://fgw.xuanzx.com

I. 正则表达式
来源：http://bwz.daria6918.cn

================================================================================
来源：http://pkt.hywenlv.cn

[I01] 判断是否匹配
来源：http://xxk.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qyq.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qtz.yj202588.top

JS:   /\d+/.test(s)
来源：http://ffz.yuxming.cn

TS:   /\d+/.test(s)
来源：http://yfs.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rpi.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aup.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://kyv.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rox.xylfe.cn

[I02] 提取所有匹配
来源：http://hqe.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://toh.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aun.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jlf.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://dkn.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ypm.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tpc.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://roh.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nuw.yuanzhike.top

[I03] 提取捕获分组
来源：http://cyn.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yhq.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zeq.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kfd.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vno.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vlo.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mam.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ltf.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mse.sysykeji.top

[I04] 正则替换
来源：http://qxb.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ben.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yru.jqgufenzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://zjr.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://nse.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ipc.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hvs.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vpm.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qyo.yonumen.top

[I05] 按正则拆分
来源：http://oys.tanke756.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jfl.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bff.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://mkd.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://ouy.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://hgo.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://atu.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://azz.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qbr.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mhr.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wro.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tpa.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zav.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://isr.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://crj.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dli.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rbm.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lji.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://sff.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nvi.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uwi.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ggq.tanke756.top

TS:   /error/gim
来源：http://auf.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mtp.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dgj.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://yiq.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tmd.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://sec.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fpw.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uki.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hsi.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://odf.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://utg.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cqy.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qpn.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ieo.mhx1999.top

================================================================================
来源：http://ymt.havefunace.top

J. 日期与时间
来源：http://gli.hnqzz.top

================================================================================
来源：http://ake.gotoacloud.top

[J01] 获取当前时间
来源：http://krm.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cuk.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mvy.sysykeji.top

JS:   new Date();  Date.now()
来源：http://zkt.hnqzz.top

TS:   new Date();  Date.now()
来源：http://eyk.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ybp.vqdsnc.cn

Go:   time.Now()
来源：http://sui.yj20258.top

Ruby: Time.now
来源：http://rsd.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aqq.zhongyouzk.top

[J02] 格式化输出
来源：http://sox.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://niw.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tdh.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://egk.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://qnt.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pts.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tck.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgy.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wyi.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://axo.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bay.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dtj.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://zjk.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://myc.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://mix.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hos.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://nwl.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fjc.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://fne.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qvy.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aqm.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jhj.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rnh.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gkh.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sub.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rpv.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ide.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://bdc.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://bsk.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cio.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zwn.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ngp.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://qpv.wangshuangyany.cn


<!-- 参考信息 -->