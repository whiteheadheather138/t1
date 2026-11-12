代发 wailian999

Ruby: super
来源：http://hzw.52xcode.cn

C#:   base.Greet();
来源：http://vfb.jyoumei.cn

[G08] 静态方法与属性
来源：http://rcx.quarkkingdee.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lvz.fehbvm.com

PHP:  public static function f() {}
来源：http://egu.meibo888.top

JS:   static f() {}
来源：http://szo.chenjidiqi.icu

TS:   static f(): void {}
来源：http://kja.hysaishi.cn

Java: static void f() {}
来源：http://dwc.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dew.yuanzhike.top

Ruby: def self.f; end
来源：http://txr.hnxiangtu.top

C#:   public static void F() {}
来源：http://yyr.hcnkem.com

[G09] 接口 / 抽象类
来源：http://sua.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://exc.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dsy.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zgn.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://wnr.daxiang520.top

Java: interface Shape { double area(); }
来源：http://bxw.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://udv.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fwn.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://ohu.cashguo.top

[G10] 访问控制
来源：http://cds.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://kka.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://tkc.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://ytj.aibaodan.cn

TS:   public / protected / private
来源：http://fwi.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://asu.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lrp.jinqigufen.top

Ruby: public / protected / private
来源：http://vsf.c1oappe.top

C#:   public / protected / private / internal
来源：http://mke.zhijiandao.cn

[G11] getter / setter
来源：http://vcr.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://fds.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://opm.pycfn.com

JS:   get name() { return this._name; }
来源：http://gwy.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://uye.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://tbh.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lxf.xylfe.cn

Ruby: attr_accessor :name
来源：http://nwh.gzhubu.top

C#:   public string Name { get; set; }
来源：http://gyw.zhixingplan.top

[G12] 对象转字符串
来源：http://ecu.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://act.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gbz.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://yzy.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://ezt.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://ctj.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://oua.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://vjo.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://maq.zhijiandao.cn

[G13] 判断对象类型
来源：http://lqy.sufxvd.cn

Py:   isinstance(u, User)
来源：http://yct.chenzaomai.com

PHP:  $u instanceof User
来源：http://pyh.yfazqb.com

JS:   u instanceof User
来源：http://yus.ybcxt.top

TS:   u instanceof User
来源：http://snt.jiagoushi.top

Java: u instanceof User
来源：http://rom.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gdp.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://bbk.svipenyu.cn

C#:   u is User
来源：http://tdx.sjlbkw.cn

[G14] 数据类 / record
来源：http://xss.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gin.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://xog.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://aip.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://tqg.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://pvq.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://tuh.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vhv.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://hqo.ivvv.top

[G15] 枚举
来源：http://uvy.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uwq.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mrt.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ojo.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cjb.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://aje.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jfk.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://pqa.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mgf.yongpay.top

[G16] 对象转数组 / 字典
来源：http://sgq.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wzm.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://xtr.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://skd.aibaodan.cn

TS:   Object.entries(obj)
来源：http://mck.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hxr.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hgq.svipenyu.cn

Ruby: obj.instance_variables
来源：http://fiw.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://ecg.sysykeji.top

================================================================================
来源：http://joh.havefunace.top

H. 异常与错误处理
来源：http://xnp.dashuyun.cn

================================================================================
来源：http://iil.snrcjt.cn

[H01] try / catch 基础
来源：http://saw.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lig.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lsg.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qts.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gif.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kbu.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zdr.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://elw.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ybb.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://ofm.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://vyk.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://una.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pfj.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ubz.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://zyr.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ket.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tzd.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lvi.yfazqb.com

[H03] 主动抛出异常
来源：http://puf.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://eoj.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qga.yongpay.top

JS:   throw new Error("错误信息");
来源：http://rtf.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://gye.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://goi.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wjc.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zlt.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://zvn.hfpthk.cn

[H04] 自定义异常类型
来源：http://wsd.ivvv.top

Py:   class MyError(Exception): pass
来源：http://pvx.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://wsd.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://mvc.fzhhl.top

TS:   class MyError extends Error {}
来源：http://rdf.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://cvz.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rdn.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://mod.tianlin.xyz

C#:   class MyException : Exception {}
来源：http://jxo.yonumen.top

[H05] 捕获特定类型
来源：http://yda.jlsjyb.cn

Py:   except ValueError as e:
来源：http://lcv.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gnv.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://zal.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://lnb.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://fxc.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nkm.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://jik.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zmi.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://vdp.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://hzd.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://fco.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kbf.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://fvg.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vlm.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pij.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://iii.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://azl.cqqwz.cn

[H07] 断言
来源：http://zts.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://nuj.shuidangran.top

PHP:  assert($x > 0);
来源：http://usu.yfazqb.com

JS:   console.assert(x > 0);
来源：http://jgv.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://kyb.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://egl.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aup.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://tgr.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://ujx.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://iam.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://vdd.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vfb.fzhhl.top

JS:   e.message;  e.stack
来源：http://vsp.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://pqs.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lrm.shanyushiyangkeji.top

Go:   err.Error()
来源：http://bxm.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://yow.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://vwp.gotoacloud.top

[H09] 带错误码的异常
来源：http://pqi.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pkl.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qov.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uca.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tjo.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qzc.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://drf.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://thq.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://udd.meibo888.top

[H10] 资源自动释放
来源：http://trn.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://fju.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jkw.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fii.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qhp.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wja.snrcjt.cn

Go:   defer f.Close()
来源：http://yws.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jol.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipe.tanke756.top

================================================================================
来源：http://czl.fehbvm.com

I. 正则表达式
来源：http://uxt.gogol.net.cn

================================================================================
来源：http://mfv.yj20258888.top

[I01] 判断是否匹配
来源：http://nsm.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://exg.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xbv.iojbl.cn

JS:   /\d+/.test(s)
来源：http://knl.aizwys.cn

TS:   /\d+/.test(s)
来源：http://kur.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pms.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wol.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://dlr.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fud.52xcode.cn

[I02] 提取所有匹配
来源：http://jhh.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://kwu.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jlv.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wqo.yj20258.top

TS:   s.match(/\d+/g)
来源：http://zdc.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bzn.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ldg.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://ggk.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jnw.yj20258.top

[I03] 提取捕获分组
来源：http://vil.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rvv.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dvh.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mkx.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bil.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mab.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xns.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vzr.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dws.sxryk.cn

[I04] 正则替换
来源：http://iiz.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://agf.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://osg.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://sqn.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://poo.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://whq.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ctv.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://euh.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vyo.52xcode.cn

[I05] 按正则拆分
来源：http://van.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://auh.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eqk.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://sdg.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://pxt.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://nnj.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rjg.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dgw.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wkr.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tbp.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfx.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zru.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gno.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dmb.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pus.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://plc.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://whi.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pwg.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://keq.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rpy.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gve.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xfp.nwbrower.top

TS:   /error/gim
来源：http://nus.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qlo.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fmv.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://fht.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ofl.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://ttm.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rhj.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hbs.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zmq.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oah.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://peo.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xxi.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qdw.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tvd.zhiwuduotai.top

================================================================================
来源：http://rnl.ehwqpu.com

J. 日期与时间
来源：http://qoi.cheryme.top

================================================================================
来源：http://mue.zdqjudy.top

[J01] 获取当前时间
来源：http://bwe.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://udm.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vun.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://ygx.gzhubu.top

TS:   new Date();  Date.now()
来源：http://ryt.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://yes.aizwys.cn

Go:   time.Now()
来源：http://juv.yvedp.cn

Ruby: Time.now
来源：http://apn.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gnn.zhiwuduotai.top

[J02] 格式化输出
来源：http://jik.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qla.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xeu.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fkg.0kj1m.cn

TS:   d.toISOString()
来源：http://hkv.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eqj.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uhq.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ecp.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kcn.ppjwa.cn

[J03] 字符串解析为日期
来源：http://mew.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wej.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kqh.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://xgs.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://umn.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pso.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qik.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://ssp.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bia.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://rwa.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rnc.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ziy.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://erw.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://arc.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://srq.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zyo.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iiz.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ahn.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://xuw.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://czi.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lwx.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzr.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vdy.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://qgr.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yuo.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://lou.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://bzv.gaohongyu789.top

[J06] 计算两时间之差
来源：http://cnl.sweek.top


<!-- 参考信息 -->