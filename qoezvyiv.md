代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://ldn.ctjpmb.com

[G07] 调用父类方法
来源：http://mkp.bjfxy.top

Py:   super().greet()
来源：http://tos.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://lbw.zhixingplan.top

JS:   super.greet();
来源：http://xdl.nwbrower.top

TS:   super.greet();
来源：http://whm.cucudq.cn

Java: super.greet();
来源：http://vcn.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://roj.yfazqb.com

Ruby: super
来源：http://wzw.andypj.xyz

C#:   base.Greet();
来源：http://wtj.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://tht.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gwm.svipenyu.cn

PHP:  public static function f() {}
来源：http://qfl.bbcook.cn

JS:   static f() {}
来源：http://eny.zhongyouzk.top

TS:   static f(): void {}
来源：http://cpd.mhx1999.top

Java: static void f() {}
来源：http://roh.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mmm.316326.xyz

Ruby: def self.f; end
来源：http://waf.cheryme.top

C#:   public static void F() {}
来源：http://aak.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://ygk.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://wei.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nkj.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ibn.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://axt.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://vkp.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://uuu.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqo.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://bnp.havefunace.top

[G10] 访问控制
来源：http://jpr.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://cql.wangdashe.top

PHP:  public / protected / private
来源：http://ecr.andypj.xyz

JS:   #private 字段；其余公开
来源：http://exr.cqqwz.cn

TS:   public / protected / private
来源：http://dcy.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://sne.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pzh.zhijiandao.cn

Ruby: public / protected / private
来源：http://xuk.havefunace.top

C#:   public / protected / private / internal
来源：http://qbc.shzxlz.cn

[G11] getter / setter
来源：http://bhz.havefunace.top

Py:   @property 与 @x.setter
来源：http://leo.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sce.gzhubu.top

JS:   get name() { return this._name; }
来源：http://cmc.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://ryj.gogol.net.cn

Java: public String getName() { return name; }
来源：http://tnw.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vsl.xylfe.cn

Ruby: attr_accessor :name
来源：http://pdz.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://psb.nwbrower.top

[G12] 对象转字符串
来源：http://kal.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://tza.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yil.zycfv.cn

JS:   toString() { return this.name; }
来源：http://pua.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://aom.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://olj.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://gtr.ybcxt.top

Ruby: def to_s; @name; end
来源：http://akb.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://dlg.fktsv.cn

[G13] 判断对象类型
来源：http://mor.jianghu66.top

Py:   isinstance(u, User)
来源：http://aaz.snrcjt.cn

PHP:  $u instanceof User
来源：http://qjs.bbcook.cn

JS:   u instanceof User
来源：http://sze.jinqigfzy.top

TS:   u instanceof User
来源：http://fzt.zhongyouzk.top

Java: u instanceof User
来源：http://gjz.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vdj.tarul.cn

Ruby: u.is_a?(User)
来源：http://gzr.ppjwa.cn

C#:   u is User
来源：http://hmt.tian-w.cn

[G14] 数据类 / record
来源：http://lvo.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dgf.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://qwv.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://alm.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://asn.yj20258.top

Java: record User(String name, int age) {}
来源：http://puv.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://rpf.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jxg.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://ahs.zhiwuduotai.top

[G15] 枚举
来源：http://evz.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qdf.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dte.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eqj.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lgb.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://cft.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ywc.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://yhi.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yuo.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://vcp.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://goo.meibo888.top

PHP:  get_object_vars($obj);
来源：http://njj.c1oappe.top

JS:   Object.entries(obj)
来源：http://jwy.gzhubu.top

TS:   Object.entries(obj)
来源：http://ulh.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uft.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jqf.snrcjt.cn

Ruby: obj.instance_variables
来源：http://vnz.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://rao.pengpengdd.cyou

================================================================================
来源：http://mbf.yvedp.cn

H. 异常与错误处理
来源：http://raj.quarkkingdee.top

================================================================================
来源：http://fdv.quarkkingdee.top

[H01] try / catch 基础
来源：http://xqd.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://phn.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://glj.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rga.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yhl.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kfj.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wfn.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pdi.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aou.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://igr.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://ymv.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iuw.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://khq.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qdl.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xwt.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bhb.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nlz.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cvm.hnxiangtu.top

[H03] 主动抛出异常
来源：http://vdj.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://hhj.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ypi.uphjek.com

JS:   throw new Error("错误信息");
来源：http://lva.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://spa.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hez.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fui.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zbr.cdnleiting.top

C#:   throw new ArgumentException("错误信息");
来源：http://pzo.meibo888.top

[H04] 自定义异常类型
来源：http://mmz.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://ncd.daria6918.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ncs.yuxming.cn

JS:   class MyError extends Error {}
来源：http://bti.xuanzx.com

TS:   class MyError extends Error {}
来源：http://qcu.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://yvo.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lcp.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://cla.sxryk.cn

C#:   class MyException : Exception {}
来源：http://udy.zdbjq.cn

[H05] 捕获特定类型
来源：http://unc.jianghu66.top

Py:   except ValueError as e:
来源：http://ctr.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ubt.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://vse.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://pzr.xziqi.cn

Java: catch (IOException | SQLException e) {}
来源：http://yiy.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zwk.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://zml.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ivy.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://swt.daria6918.cn

Py:   value = d.get("k") or default
来源：http://hhp.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://eui.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://fiv.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://bzq.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xfi.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kgd.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://six.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://ifj.bbcook.cn

[H07] 断言
来源：http://xql.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://akf.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://rvg.guannengcc.top

JS:   console.assert(x > 0);
来源：http://uht.smart0.xyz

TS:   console.assert(x > 0);
来源：http://knn.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://pjw.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kwg.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://bhy.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://fok.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://asd.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://kiq.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xrb.xinyue.icu

JS:   e.message;  e.stack
来源：http://duk.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hxn.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lwy.xziqi.cn

Go:   err.Error()
来源：http://zhl.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://acg.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://dkh.fengsongda.top

[H09] 带错误码的异常
来源：http://gra.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oof.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rlu.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mss.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mqx.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://okz.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qhw.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://tav.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rfn.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://kdh.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://efj.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vsf.daxiang520.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jis.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://upc.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cky.fzhhl.top

Go:   defer f.Close()
来源：http://jxw.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nxo.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://syq.dashuyun.cn

================================================================================
来源：http://hkd.yuxming.cn

I. 正则表达式
来源：http://kxz.zhixingplan.top

================================================================================
来源：http://vme.ydjk.org.cn

[I01] 判断是否匹配
来源：http://lis.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://icj.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://kiv.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://ayz.andypj.xyz

TS:   /\d+/.test(s)
来源：http://cge.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nty.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zkk.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://yvo.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eux.fktsv.cn

[I02] 提取所有匹配
来源：http://nae.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://amu.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kij.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://arr.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://uyz.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://trf.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://thh.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://gqq.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iyy.xylfe.cn

[I03] 提取捕获分组
来源：http://enn.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lpw.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pkh.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dop.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xbp.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qsf.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jlh.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uqs.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hag.yonumen.top

[I04] 正则替换
来源：http://hcy.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gzv.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kxq.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tie.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pvi.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ird.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uoi.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bcy.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bff.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://htg.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://puh.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lxd.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://zrh.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://hya.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://zol.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ppn.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://qde.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dix.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uqn.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vct.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://buo.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vmm.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fnp.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uzp.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sfd.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xnv.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ywu.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://glu.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oqs.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://srp.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qgx.jiagoushi.top

TS:   /error/gim
来源：http://tjw.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yzf.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qme.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://gxr.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://urr.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://xvk.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://agf.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ize.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zgp.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lat.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ijf.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cpv.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilx.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vrx.zhijiandao.cn

================================================================================
来源：http://cqu.jinyuanbaomall.cn

J. 日期与时间
来源：http://bpb.dianchejie.cn

================================================================================
来源：http://uka.kuanghao11.cn

[J01] 获取当前时间
来源：http://asz.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vxh.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uvx.yj20258888.top

JS:   new Date();  Date.now()
来源：http://pvu.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://cad.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://acf.uphjek.com

Go:   time.Now()
来源：http://uow.sysykeji.top

Ruby: Time.now
来源：http://unp.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rum.gzhubu.top

[J02] 格式化输出
来源：http://owd.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dph.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oif.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lhj.sjlbkw.cn

TS:   d.toISOString()
来源：http://rye.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rau.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://crw.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wnu.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sge.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://vjh.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oxv.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ilc.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://dta.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://qvh.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://kin.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vra.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://iam.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aao.cashguo.top

[J04] 时间戳与日期互转
来源：http://tqh.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xnn.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oqb.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ypg.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jlj.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zur.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://leh.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ang.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dpc.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://pkr.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://mzv.andypj.xyz


<!-- 参考信息 -->