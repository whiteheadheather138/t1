代发 wailian999

JS:   super.greet();
来源：http://nsb.ivvv.top

TS:   super.greet();
来源：http://wap.chenjidiqi.icu

Java: super.greet();
来源：http://zef.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wlv.cqqwz.cn

Ruby: super
来源：http://xrs.svipenyu.cn

C#:   base.Greet();
来源：http://vmc.hnxiangtu.top

[G08] 静态方法与属性
来源：http://nno.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hjh.cheryme.top

PHP:  public static function f() {}
来源：http://rmo.c1oappe.top

JS:   static f() {}
来源：http://lck.jqgufenzy.top

TS:   static f(): void {}
来源：http://ryw.jinyuanbaomall.cn

Java: static void f() {}
来源：http://fdu.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://she.sxryk.cn

Ruby: def self.f; end
来源：http://lwc.cucudq.cn

C#:   public static void F() {}
来源：http://xao.birdmap.top

[G09] 接口 / 抽象类
来源：http://kgq.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://ulj.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://kdk.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yil.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://pxg.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://xpc.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://vca.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jxm.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://nxx.shangyingyoupin.top

[G10] 访问控制
来源：http://ouf.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://xxi.zhijiandao.cn

PHP:  public / protected / private
来源：http://fur.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://ite.jinqigfzy.top

TS:   public / protected / private
来源：http://ipg.cheryme.top

Java: public / protected / private / 默认包级
来源：http://oto.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://apm.svipenyu.cn

Ruby: public / protected / private
来源：http://ahr.zdbjq.cn

C#:   public / protected / private / internal
来源：http://dlo.ctjpmb.com

[G11] getter / setter
来源：http://iet.vehdjk.com

Py:   @property 与 @x.setter
来源：http://hxr.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://sxy.zycfv.cn

JS:   get name() { return this._name; }
来源：http://yca.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://led.vehdjk.com

Java: public String getName() { return name; }
来源：http://tsa.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yda.snrcjt.cn

Ruby: attr_accessor :name
来源：http://ibq.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://geq.316326.xyz

[G12] 对象转字符串
来源：http://vjr.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://uoc.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://cnn.mhx1999.top

JS:   toString() { return this.name; }
来源：http://zqo.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://yvc.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://ksn.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://qca.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://avk.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://biy.zhoulong.xyz

[G13] 判断对象类型
来源：http://wxv.andypj.xyz

Py:   isinstance(u, User)
来源：http://xik.bjfxy.top

PHP:  $u instanceof User
来源：http://lro.nanxuanxn.top

JS:   u instanceof User
来源：http://gpe.ybcxt.top

TS:   u instanceof User
来源：http://cvz.dashuyun.cn

Java: u instanceof User
来源：http://vpw.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iil.bbcook.cn

Ruby: u.is_a?(User)
来源：http://afb.ywan-chungtsiang.top

C#:   u is User
来源：http://jol.chenjidiqi.icu

[G14] 数据类 / record
来源：http://jaj.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://avm.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://dza.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://tle.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://wfj.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://hby.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://aet.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rsf.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://pvg.tarul.cn

[G15] 枚举
来源：http://lic.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kde.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xto.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ttp.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sbl.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://eyl.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://onh.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://bpe.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://els.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://xta.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wzv.shanyushiyangkeji.top

PHP:  get_object_vars($obj);
来源：http://wyw.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://twb.xziqi.cn

TS:   Object.entries(obj)
来源：http://zxz.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lfg.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jks.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://chs.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://kra.ydjk.org.cn

================================================================================
来源：http://ajr.hnqzz.top

H. 异常与错误处理
来源：http://ryr.shzxlz.cn

================================================================================
来源：http://niy.yuanzhike.top

[H01] try / catch 基础
来源：http://djs.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qft.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ohx.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xsq.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pmd.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ouz.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oec.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gkt.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://npt.hammf.cn

[H02] finally / ensure 收尾
来源：http://ncy.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oxw.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nhm.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wad.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gab.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://dgs.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rhy.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nfk.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ybr.dianchejie.cn

[H03] 主动抛出异常
来源：http://dib.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://pzv.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vyz.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://jgs.cashguo.top

TS:   throw new Error("错误信息");
来源：http://wfs.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqk.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rpw.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kgy.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://aig.chenlongwang.top

[H04] 自定义异常类型
来源：http://gjc.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://aft.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://vtg.fzhhl.top

JS:   class MyError extends Error {}
来源：http://hwm.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://mfj.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://xui.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jse.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://isn.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://tkf.yonumen.top

[H05] 捕获特定类型
来源：http://qit.shuidangran.top

Py:   except ValueError as e:
来源：http://gcd.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dry.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://ffk.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://cso.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://llv.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qly.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://zbz.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yia.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://dfr.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://xwv.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://toh.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fmx.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eqx.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vpb.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tsg.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://oqk.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://ehk.havefunace.top

[H07] 断言
来源：http://qix.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://fda.wangdashe.top

PHP:  assert($x > 0);
来源：http://oxs.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://dzk.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://mwu.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://kjy.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rta.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://deu.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://viu.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://tqt.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://tgf.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jil.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://zkb.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rxk.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pmx.redwolf501.top

Go:   err.Error()
来源：http://bed.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://qic.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://uqc.yuxming.cn

[H09] 带错误码的异常
来源：http://hbu.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpn.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://slv.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vxg.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgc.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pao.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jci.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://ulg.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ipd.hammf.cn

[H10] 资源自动释放
来源：http://tep.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rgj.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qui.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fvf.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ryq.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lwr.cashguo.top

Go:   defer f.Close()
来源：http://iiy.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ibp.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://msz.jyoumei.cn

================================================================================
来源：http://nxm.hfpthk.cn

I. 正则表达式
来源：http://fva.jianghu66.top

================================================================================
来源：http://rsk.yuxming.cn

[I01] 判断是否匹配
来源：http://wpy.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://imu.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://ozx.birdmap.top

JS:   /\d+/.test(s)
来源：http://gtn.andypj.xyz

TS:   /\d+/.test(s)
来源：http://sht.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iux.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rvk.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://lew.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lht.shzxlz.cn

[I02] 提取所有匹配
来源：http://vrr.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://ypn.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wmm.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://owa.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://tpv.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://chi.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vkw.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://ylu.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hvr.zhongyouzk.top

[I03] 提取捕获分组
来源：http://evp.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qte.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qpq.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yfv.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ubn.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://haj.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yub.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gxh.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ser.chenzaomai.com

[I04] 正则替换
来源：http://zmi.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vpu.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqz.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://ajz.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://fns.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://syb.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://uns.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xcb.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vfb.yueranfly.top

[I05] 按正则拆分
来源：http://wvn.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oqx.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hxp.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://zih.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://pee.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://xzj.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ncb.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rkh.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hvo.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fha.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wbq.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wmw.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vco.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xlo.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zab.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xus.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hlb.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kxj.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://dqq.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ius.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vac.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wlb.fengsongda.top

TS:   /error/gim
来源：http://wjo.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jzg.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tba.havefunace.top

Ruby: s.scan(/error/i)
来源：http://zny.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yjq.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://cfi.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://owx.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zxp.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gse.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffs.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgn.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://irt.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rni.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iwc.redwolf501.top

================================================================================
来源：http://ryx.316326.xyz

J. 日期与时间
来源：http://jgd.iojbl.cn

================================================================================
来源：http://xum.svipenyu.cn

[J01] 获取当前时间
来源：http://txy.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cgm.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pvp.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://bnu.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://sbe.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://juq.aibaodan.cn

Go:   time.Now()
来源：http://jqw.tarul.cn

Ruby: Time.now
来源：http://msn.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vlu.guannengcc.top

[J02] 格式化输出
来源：http://lhe.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cjj.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fcc.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dmo.hnqzz.top

TS:   d.toISOString()
来源：http://wvx.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ico.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mzz.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pxh.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ciy.jqgfzy.top

[J03] 字符串解析为日期
来源：http://rxe.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xkc.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://csg.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://lxd.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://khi.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nnh.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pla.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://bnz.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://upn.yuxming.cn

[J04] 时间戳与日期互转
来源：http://hno.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bsn.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://svv.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hkq.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ewi.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uvw.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oss.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iys.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yje.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://yps.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://ptr.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gmq.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gsj.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wbv.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://fyo.zycfv.cn


<!-- 参考信息 -->