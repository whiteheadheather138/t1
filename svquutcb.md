代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://iuq.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://tar.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dmt.yongpay.top

Ruby: def greet; "admin"; end
来源：http://zcg.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://gjy.dashuyun.cn

[G07] 调用父类方法
来源：http://gjg.daria6918.cn

Py:   super().greet()
来源：http://kha.hongshengwenyu.top

PHP:  parent::greet();
来源：http://ggx.fzhhl.top

JS:   super.greet();
来源：http://tln.shanyushiyangkeji.top

TS:   super.greet();
来源：http://amk.jianghu66.top

Java: super.greet();
来源：http://ldp.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://syy.xinyue.icu

Ruby: super
来源：http://tmm.gzhubu.top

C#:   base.Greet();
来源：http://prd.meibo888.top

[G08] 静态方法与属性
来源：http://zyt.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qbo.ivvv.top

PHP:  public static function f() {}
来源：http://jxi.ctjpmb.com

JS:   static f() {}
来源：http://ttj.mhx1999.top

TS:   static f(): void {}
来源：http://zwb.yvedp.cn

Java: static void f() {}
来源：http://wkw.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://sfn.chenzaomai.com

Ruby: def self.f; end
来源：http://kjt.xziqi.cn

C#:   public static void F() {}
来源：http://ubk.52xcode.cn

[G09] 接口 / 抽象类
来源：http://bls.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://kfj.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eqs.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wkr.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://vct.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://pgw.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://rgu.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fzz.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://bhx.nanxuanxn.top

[G10] 访问控制
来源：http://dtn.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://whg.nanxuanxn.top

PHP:  public / protected / private
来源：http://oit.yvedp.cn

JS:   #private 字段；其余公开
来源：http://pkb.zhengqikj.top

TS:   public / protected / private
来源：http://kbt.ivvv.top

Java: public / protected / private / 默认包级
来源：http://tit.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://aqc.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://wce.tianlin.xyz

C#:   public / protected / private / internal
来源：http://vqx.smart0.xyz

[G11] getter / setter
来源：http://deq.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://oab.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://htv.yueranfly.top

JS:   get name() { return this._name; }
来源：http://rba.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://bzg.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://hpt.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gpy.fengsongda.top

Ruby: attr_accessor :name
来源：http://yzf.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://uxw.tian-w.cn

[G12] 对象转字符串
来源：http://qpo.tanke756.top

Py:   def __str__(self): return self.name
来源：http://rud.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://dgo.zycfv.cn

JS:   toString() { return this.name; }
来源：http://una.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://zal.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://njt.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uey.yj20258888.top

Ruby: def to_s; @name; end
来源：http://soa.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://qvh.redwolf501.top

[G13] 判断对象类型
来源：http://hju.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://wat.birdmap.top

PHP:  $u instanceof User
来源：http://xas.tanke756.top

JS:   u instanceof User
来源：http://own.shzxlz.cn

TS:   u instanceof User
来源：http://crk.cucudq.cn

Java: u instanceof User
来源：http://bwx.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dyd.tanke756.top

Ruby: u.is_a?(User)
来源：http://gdk.gaohongyu789.top

C#:   u is User
来源：http://axx.yvedp.cn

[G14] 数据类 / record
来源：http://cve.pycfn.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eky.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://wjv.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://xbl.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://cbk.daxiang520.top

Java: record User(String name, int age) {}
来源：http://tuw.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://wyj.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cey.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://vvf.tanke756.top

[G15] 枚举
来源：http://sjd.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ydb.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pqc.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nti.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uoa.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://pfx.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dpx.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://rao.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pud.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://dpx.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gdl.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://wnj.aizwys.cn

JS:   Object.entries(obj)
来源：http://fkf.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://olm.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://huw.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ixy.snrcjt.cn

Ruby: obj.instance_variables
来源：http://tca.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://ehd.zdqjudy.top

================================================================================
来源：http://mpc.shangyingyoupin.top

H. 异常与错误处理
来源：http://cug.cdnleiting.top

================================================================================
来源：http://iqz.wangshuangyany.cn

[H01] try / catch 基础
来源：http://kpw.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ipa.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dfn.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://moc.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ubc.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iin.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://obs.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kki.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yox.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://kcs.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://lrb.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ice.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://xrv.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ird.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uoi.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://krj.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fyf.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vuk.pycfn.com

[H03] 主动抛出异常
来源：http://svt.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://qvh.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kes.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://hbn.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://vuc.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vxk.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ave.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aul.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vud.svipenyu.cn

[H04] 自定义异常类型
来源：http://gvd.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://oer.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pmn.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://wua.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://poh.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://qfa.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://amm.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://xmb.sxryk.cn

C#:   class MyException : Exception {}
来源：http://orh.wangdashe.top

[H05] 捕获特定类型
来源：http://cvq.xylfe.cn

Py:   except ValueError as e:
来源：http://jyq.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://puw.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://qob.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://tuo.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://dwp.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ptx.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://oal.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vqn.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://qob.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://ckv.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://bvu.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://hcq.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bdw.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jcj.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pqy.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://aey.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://cze.smart0.xyz

[H07] 断言
来源：http://bci.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://utv.cucudq.cn

PHP:  assert($x > 0);
来源：http://mxf.daxiang520.top

JS:   console.assert(x > 0);
来源：http://szw.yongpay.top

TS:   console.assert(x > 0);
来源：http://hzl.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://kdj.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hwt.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://nin.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://phq.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://sho.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://pyh.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zem.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://tba.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ewd.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mdn.iojbl.cn

Go:   err.Error()
来源：http://snk.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://zxp.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://kwz.ehwqpu.com

[H09] 带错误码的异常
来源：http://rla.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tcy.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qdy.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sbv.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fqz.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iio.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ubo.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://coz.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://dfu.yongpay.top

[H10] 资源自动释放
来源：http://obs.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tyn.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tyj.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eow.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nix.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uam.epnwcf.com

Go:   defer f.Close()
来源：http://xyb.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://unm.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cey.wangdashe.top

================================================================================
来源：http://pjr.feifeiyinyue.top

I. 正则表达式
来源：http://gpu.hnqzz.top

================================================================================
来源：http://uwu.dashuyun.cn

[I01] 判断是否匹配
来源：http://cpk.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jyt.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://iwr.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://kpj.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://ogc.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hra.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://frx.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://nly.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wny.jqgfzy.top

[I02] 提取所有匹配
来源：http://var.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://biv.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hgb.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gpu.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://etg.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fcm.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xvc.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://kis.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lbg.zhixingplan.top

[I03] 提取捕获分组
来源：http://jxp.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gpd.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pmw.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gui.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cdy.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ind.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://guq.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pus.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dxk.jinqigufen.top

[I04] 正则替换
来源：http://jsa.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ffm.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lhg.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://opx.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ahf.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bne.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wko.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://jew.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hsq.wangdashe.top

[I05] 按正则拆分
来源：http://ilf.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bkn.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsv.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://waf.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://gin.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://fdf.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jpr.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://ogd.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rnl.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zuk.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jgt.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yra.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzk.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msc.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ibo.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sfx.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pdt.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://woz.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://ebb.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hmn.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lne.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://plq.ehwqpu.com

TS:   /error/gim
来源：http://htt.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sda.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xwp.tarul.cn

Ruby: s.scan(/error/i)
来源：http://gps.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wua.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://www.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://amp.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://omw.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hrs.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmi.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lba.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eny.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://duo.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://piv.hywenlv.cn

================================================================================
来源：http://ofe.feifeiyinyue.top

J. 日期与时间
来源：http://igx.chenlongwang.top

================================================================================
来源：http://frl.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://eki.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cfo.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uwp.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://evv.tian-w.cn

TS:   new Date();  Date.now()
来源：http://qda.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://htc.sufxvd.cn

Go:   time.Now()
来源：http://xnq.zycfv.cn

Ruby: Time.now
来源：http://jbt.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zen.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://sms.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qwm.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fmm.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uag.jiagoushi.top

TS:   d.toISOString()
来源：http://frq.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pij.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://atw.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aun.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://njr.zdqjudy.top

[J03] 字符串解析为日期
来源：http://oqb.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tcr.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xjv.316326.xyz

JS:   new Date("2024-01-02")
来源：http://abh.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://geg.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://ndh.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xkg.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://syk.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yvz.smart0.xyz

[J04] 时间戳与日期互转
来源：http://maw.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wxp.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://luk.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cjp.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ilc.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aoi.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ztm.zhoulong.xyz


<!-- 参考信息 -->