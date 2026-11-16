代发 wailian999

[G06] 重写方法
来源：http://hos.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://ctn.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jtu.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://sko.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://mxw.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://klw.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iof.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://wgt.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://cys.jiagoushi.top

[G07] 调用父类方法
来源：http://acx.yj202588.top

Py:   super().greet()
来源：http://dia.jianghu66.top

PHP:  parent::greet();
来源：http://hvv.mhx1999.top

JS:   super.greet();
来源：http://lri.jiagoushi.top

TS:   super.greet();
来源：http://wra.svipenyu.cn

Java: super.greet();
来源：http://hnf.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bxw.zdqjudy.top

Ruby: super
来源：http://iak.jianghu66.top

C#:   base.Greet();
来源：http://ufc.aizwys.cn

[G08] 静态方法与属性
来源：http://xtq.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gbx.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://xgu.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://ncu.daria6918.cn

TS:   static f(): void {}
来源：http://trr.0kj1m.cn

Java: static void f() {}
来源：http://wcr.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xap.jiagoushi.top

Ruby: def self.f; end
来源：http://bxb.gogol.net.cn

C#:   public static void F() {}
来源：http://rvw.aizwys.cn

[G09] 接口 / 抽象类
来源：http://fyl.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://gtf.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://bwh.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pxh.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://aqb.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://rry.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://ina.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jzk.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://dmz.hesvh.cn

[G10] 访问控制
来源：http://xvq.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://qsy.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://orr.smart0.xyz

JS:   #private 字段；其余公开
来源：http://pfd.chenjidiqi.icu

TS:   public / protected / private
来源：http://ycl.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://xkn.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ths.c1oappe.top

Ruby: public / protected / private
来源：http://lat.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://baj.yuxming.cn

[G11] getter / setter
来源：http://scy.iojbl.cn

Py:   @property 与 @x.setter
来源：http://lye.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ecu.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://bzk.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://lrj.birdmap.top

Java: public String getName() { return name; }
来源：http://ewr.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pvp.yongpay.top

Ruby: attr_accessor :name
来源：http://zib.hnqzz.top

C#:   public string Name { get; set; }
来源：http://uuy.zycfv.cn

[G12] 对象转字符串
来源：http://pul.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://yvz.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gjq.yonumen.top

JS:   toString() { return this.name; }
来源：http://rcf.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://hwr.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://bwu.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fte.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://icw.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://cow.cheryme.top

[G13] 判断对象类型
来源：http://aun.yj20258888.top

Py:   isinstance(u, User)
来源：http://cju.zdbjq.cn

PHP:  $u instanceof User
来源：http://iyu.hammf.cn

JS:   u instanceof User
来源：http://cmb.ydzc1.top

TS:   u instanceof User
来源：http://dyl.hcnkem.com

Java: u instanceof User
来源：http://ypo.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://mit.316326.xyz

Ruby: u.is_a?(User)
来源：http://llf.gaohongyu789.top

C#:   u is User
来源：http://bgm.shangyingyoupin.top

[G14] 数据类 / record
来源：http://pwy.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ggi.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://wga.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lql.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://wnx.daxiang520.top

Java: record User(String name, int age) {}
来源：http://yux.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://vts.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://huj.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://hou.nanxuanxn.top

[G15] 枚举
来源：http://xfw.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xxc.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://btm.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tlq.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://and.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://uip.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ifr.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://gkg.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ofa.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://dpr.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bha.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://ybz.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://rta.hammf.cn

TS:   Object.entries(obj)
来源：http://bdb.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kvl.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sxb.bbcook.cn

Ruby: obj.instance_variables
来源：http://yst.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://uhw.yangfankeji.com

================================================================================
来源：http://nth.zdbjq.cn

H. 异常与错误处理
来源：http://fow.tianlin.xyz

================================================================================
来源：http://vaf.vehdjk.com

[H01] try / catch 基础
来源：http://kxn.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gkw.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ksw.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ywm.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xum.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vgn.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ksn.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fdw.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ssm.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://dra.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hes.chenjidiqi.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://qem.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dbz.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jep.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://yxi.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://izl.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ysi.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://zsw.yonumen.top

[H03] 主动抛出异常
来源：http://zfs.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://lly.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uie.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://ufa.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://dkf.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://smk.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yma.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xpv.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://lyk.zhoulong.xyz

[H04] 自定义异常类型
来源：http://tim.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://siz.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://ixi.52xcode.cn

JS:   class MyError extends Error {}
来源：http://ils.shuidangran.top

TS:   class MyError extends Error {}
来源：http://zpj.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://xwx.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wzd.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://bab.nwbrower.top

C#:   class MyException : Exception {}
来源：http://yfi.tian-w.cn

[H05] 捕获特定类型
来源：http://xpr.hnqzz.top

Py:   except ValueError as e:
来源：http://mke.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rei.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://gcz.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://tme.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://iho.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zcv.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://imz.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://azb.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://ekk.fengsongda.top

Py:   value = d.get("k") or default
来源：http://bld.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://izv.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://izk.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://ktc.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ikk.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gek.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://two.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://gkk.c1oappe.top

[H07] 断言
来源：http://hhm.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://ihj.jqgfzy.top

PHP:  assert($x > 0);
来源：http://edm.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://afw.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://fsy.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://mmm.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jzm.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://tcg.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://bcw.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://hlw.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://gjk.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://azo.dashuyun.cn

JS:   e.message;  e.stack
来源：http://dfy.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fwl.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://vgp.cheryme.top

Go:   err.Error()
来源：http://iac.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://vus.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://omz.yj20258888.top

[H09] 带错误码的异常
来源：http://qro.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wck.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ali.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://abp.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://emg.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fmx.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ixs.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://nbg.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xre.cqqwz.cn

[H10] 资源自动释放
来源：http://isr.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://orr.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fck.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ufb.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rll.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xji.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://ftg.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nuk.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ivt.cucudq.cn

================================================================================
来源：http://egn.jinqigufen.top

I. 正则表达式
来源：http://wdf.hywenlv.cn

================================================================================
来源：http://lvu.sxryk.cn

[I01] 判断是否匹配
来源：http://sfs.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qbw.jlsjyb.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hbl.316326.xyz

JS:   /\d+/.test(s)
来源：http://zmw.hammf.cn

TS:   /\d+/.test(s)
来源：http://paf.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tzj.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tak.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://usa.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mif.cashguo.top

[I02] 提取所有匹配
来源：http://ffw.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://xek.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://krr.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wlh.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://kxf.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aji.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vtq.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://hzv.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mpp.zhoulong.xyz

[I03] 提取捕获分组
来源：http://dyu.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://efn.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oks.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jbn.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gvc.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nbl.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tku.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sdb.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wvm.ivvv.top

[I04] 正则替换
来源：http://zid.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ipv.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wwy.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://wpt.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://eng.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://mhe.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://rml.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fuf.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zoy.nwbrower.top

[I05] 按正则拆分
来源：http://fmu.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://krf.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rzm.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://hcl.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://lnt.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://jak.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://imz.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://czc.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dne.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yze.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://znt.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rqw.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zrq.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwi.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bsk.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cdc.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nzq.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mpn.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://dfb.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sas.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cyo.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oel.yanxiufei.cn

TS:   /error/gim
来源：http://lyh.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ldl.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jpb.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://bbi.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xks.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://jiu.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://snw.bjfxy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://soh.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gih.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jal.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://etk.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tqo.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lnb.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ftd.hesvh.cn

================================================================================
来源：http://wgz.xylfe.cn

J. 日期与时间
来源：http://pyw.ybcxt.top

================================================================================
来源：http://fyh.meibo888.top

[J01] 获取当前时间
来源：http://che.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rjh.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mlw.xuanzx.com

JS:   new Date();  Date.now()
来源：http://lfc.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://bpj.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yfb.52xcode.cn

Go:   time.Now()
来源：http://zue.jlsjyb.cn

Ruby: Time.now
来源：http://usc.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zxv.sweek.top

[J02] 格式化输出
来源：http://qku.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ucr.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ftm.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uzq.c1oappe.top

TS:   d.toISOString()
来源：http://anh.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qvy.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kpg.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfc.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cmb.yueranfly.top

[J03] 字符串解析为日期
来源：http://ifw.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kxe.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lno.cheryme.top

JS:   new Date("2024-01-02")
来源：http://jvn.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://ime.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://dzs.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mun.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://bje.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zdx.hongshengwenyu.top

[J04] 时间戳与日期互转
来源：http://arz.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://evi.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tdo.yj20258.top


<!-- 参考信息 -->