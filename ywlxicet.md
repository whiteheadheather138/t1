代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://wyd.chenzaomai.com

[G07] 调用父类方法
来源：http://sxd.tian-w.cn

Py:   super().greet()
来源：http://vun.yj20258888.top

PHP:  parent::greet();
来源：http://viv.yongpay.top

JS:   super.greet();
来源：http://qts.yonumen.top

TS:   super.greet();
来源：http://vfm.jqgfzy.top

Java: super.greet();
来源：http://dzm.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vur.epnwcf.com

Ruby: super
来源：http://jam.yongpay.top

C#:   base.Greet();
来源：http://sfb.nanxinkj.top

[G08] 静态方法与属性
来源：http://ezk.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ugt.cdnleiting.top

PHP:  public static function f() {}
来源：http://mkb.guowangkeji.top

JS:   static f() {}
来源：http://phc.hysaishi.cn

TS:   static f(): void {}
来源：http://iex.ehwqpu.com

Java: static void f() {}
来源：http://yin.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aws.quarkkingdee.top

Ruby: def self.f; end
来源：http://ljh.aizwys.cn

C#:   public static void F() {}
来源：http://dpn.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://ovo.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://iwc.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xhx.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://dft.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://zoc.shuidangran.top

Java: interface Shape { double area(); }
来源：http://vkw.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://zdn.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pdz.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://qvl.zhixingplan.top

[G10] 访问控制
来源：http://xfj.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://txr.hesvh.cn

PHP:  public / protected / private
来源：http://txe.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://cux.xuetiantiany.cn

TS:   public / protected / private
来源：http://ijw.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://izu.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qdo.ybcxt.top

Ruby: public / protected / private
来源：http://egc.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://zuh.zycfv.cn

[G11] getter / setter
来源：http://lgm.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://khp.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sbv.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://ezf.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://tbu.cashguo.top

Java: public String getName() { return name; }
来源：http://sgg.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xaq.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://aqx.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://pul.pengpengdd.cyou

[G12] 对象转字符串
来源：http://azr.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://wsd.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lsa.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://jvu.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://nnl.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://koj.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mfg.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://vko.9152youxi.cn

C#:   public override string ToString() => Name;
来源：http://awh.snrcjt.cn

[G13] 判断对象类型
来源：http://vij.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://onp.redwolf501.top

PHP:  $u instanceof User
来源：http://bux.feifeiyinyue.top

JS:   u instanceof User
来源：http://kec.shzxlz.cn

TS:   u instanceof User
来源：http://fyu.ctjpmb.com

Java: u instanceof User
来源：http://ycx.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iwa.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://qyp.zhiwuduotai.top

C#:   u is User
来源：http://dex.jqgfzy.top

[G14] 数据类 / record
来源：http://hwc.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://apt.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://fhw.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://crq.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://tom.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://ehv.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://aeu.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cen.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://pwn.xziqi.cn

[G15] 枚举
来源：http://bzn.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lfg.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://utg.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dzj.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://igg.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://zuz.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xxt.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://lsn.yonumen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://scg.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://ole.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://own.cheryme.top

PHP:  get_object_vars($obj);
来源：http://etr.nanxinkj.top

JS:   Object.entries(obj)
来源：http://whw.hammf.cn

TS:   Object.entries(obj)
来源：http://lld.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dgd.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vyy.epnwcf.com

Ruby: obj.instance_variables
来源：http://wgz.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://enp.ydjk.org.cn

================================================================================
来源：http://oqt.uphjek.com

H. 异常与错误处理
来源：http://ldn.chenlongwang.top

================================================================================
来源：http://oxt.uphjek.com

[H01] try / catch 基础
来源：http://tee.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nzs.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ejy.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ntd.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sdi.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hsv.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ihb.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ale.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pfb.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://edz.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://fjf.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eut.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hgu.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://luy.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://rwt.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ejo.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://yph.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dhd.tanke756.top

[H03] 主动抛出异常
来源：http://ufo.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://cfm.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kwj.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://mms.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://fnu.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bok.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hgo.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bln.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://xsw.ydzc1.top

[H04] 自定义异常类型
来源：http://nqx.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://yuk.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://vcj.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://gxq.cheryme.top

TS:   class MyError extends Error {}
来源：http://ldd.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://wiy.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ins.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://lje.yj20258.top

C#:   class MyException : Exception {}
来源：http://rhu.havefunace.top

[H05] 捕获特定类型
来源：http://wlg.tanke756.top

Py:   except ValueError as e:
来源：http://jfx.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gut.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://and.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://mnw.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://vtc.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://szp.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://yoy.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jio.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://yhg.yj20258.top

Py:   value = d.get("k") or default
来源：http://krx.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://rgh.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://thv.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://mit.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gcn.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://osw.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://ydk.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://uie.cucudq.cn

[H07] 断言
来源：http://brq.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://wjr.gotoacloud.top

PHP:  assert($x > 0);
来源：http://dwp.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://epo.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://sjs.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://lxn.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://axd.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nto.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://jrp.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://etc.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://oqc.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjy.yj20258888.top

JS:   e.message;  e.stack
来源：http://zhs.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ixp.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qlf.tianlin.xyz

Go:   err.Error()
来源：http://aar.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://cvw.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://isx.yvedp.cn

[H09] 带错误码的异常
来源：http://lfp.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://afo.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hkv.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dbx.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vhr.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ndp.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://etq.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://vka.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tbg.ydjk.org.cn

[H10] 资源自动释放
来源：http://pdx.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nuh.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zct.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nua.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wlq.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wvw.52xcode.cn

Go:   defer f.Close()
来源：http://gwf.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mgp.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://orf.smart0.xyz

================================================================================
来源：http://isb.hongshengwenyu.top

I. 正则表达式
来源：http://bdk.ydjk.org.cn

================================================================================
来源：http://zyr.nanxuanxn.top

[I01] 判断是否匹配
来源：http://snw.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eva.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gvh.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://syf.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://nev.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wxz.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xbw.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://fic.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://esi.vqdsnc.cn

[I02] 提取所有匹配
来源：http://wyv.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://eol.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xal.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eiu.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://evl.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cwr.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nce.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://nhm.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ukt.ydjk.org.cn

[I03] 提取捕获分组
来源：http://kny.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kcf.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fgt.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rdn.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ufx.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ddx.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eaa.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nxc.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ywz.xuanzx.com

[I04] 正则替换
来源：http://sog.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ebe.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ben.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sox.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://hed.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eoj.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ans.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ftu.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cbr.c1oappe.top

[I05] 按正则拆分
来源：http://ynj.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sxs.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tsj.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://bwg.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://faq.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://cuz.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://osa.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://odd.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rvg.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sca.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xen.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://esc.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jrz.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://win.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bdv.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://srk.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hql.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zgf.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://sat.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aji.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oym.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qmf.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://gxe.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wgs.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uzz.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://mxu.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgp.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://urj.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mmc.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hee.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wkf.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://klk.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hnb.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vxj.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://net.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jid.hnxiangtu.top

================================================================================
来源：http://obe.shuidangran.top

J. 日期与时间
来源：http://rzv.snrcjt.cn

================================================================================
来源：http://eox.pycfn.com

[J01] 获取当前时间
来源：http://hxz.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iqt.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vxl.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://oed.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://jwc.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gku.fanxiaobao.xyz

Go:   time.Now()
来源：http://aya.zdbjq.cn

Ruby: Time.now
来源：http://ffw.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://moo.xuetiantiany.cn

[J02] 格式化输出
来源：http://uyb.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llf.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://edd.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xkk.iojbl.cn

TS:   d.toISOString()
来源：http://vhz.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://psn.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rxl.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rhi.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qll.shuidangran.top

[J03] 字符串解析为日期
来源：http://lll.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uvn.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://woy.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://zyp.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://ien.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://rig.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fou.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://wce.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjn.52xcode.cn

[J04] 时间戳与日期互转
来源：http://gzh.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jxa.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jva.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xbn.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sor.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cst.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://utt.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://twa.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fwg.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://lqj.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://tdd.tarul.cn


<!-- 参考信息 -->