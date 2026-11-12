代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://ngg.shangyingyoupin.top

Ruby: def self.f; end
来源：http://oya.yj202588.top

C#:   public static void F() {}
来源：http://fby.cashguo.top

[G09] 接口 / 抽象类
来源：http://mwv.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://drr.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://bad.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gvn.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://dly.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://kji.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://sbq.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zlw.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://epp.yfazqb.com

[G10] 访问控制
来源：http://rzl.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://uyj.feifeiyinyue.top

PHP:  public / protected / private
来源：http://fnk.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://lub.cdnleiting.top

TS:   public / protected / private
来源：http://ugj.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://jih.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yks.gaohongyu789.top

Ruby: public / protected / private
来源：http://lop.uphjek.com

C#:   public / protected / private / internal
来源：http://qog.aibaodan.cn

[G11] getter / setter
来源：http://tqg.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://bcj.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kos.pycfn.com

JS:   get name() { return this._name; }
来源：http://vge.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://tva.havefunace.top

Java: public String getName() { return name; }
来源：http://apv.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dqs.svipenyu.cn

Ruby: attr_accessor :name
来源：http://oml.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://nnh.zdqjudy.top

[G12] 对象转字符串
来源：http://nvx.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://dif.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rvp.tanke756.top

JS:   toString() { return this.name; }
来源：http://jfy.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://afm.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://anc.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://pgl.sweek.top

Ruby: def to_s; @name; end
来源：http://udt.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://nig.yongpay.top

[G13] 判断对象类型
来源：http://zax.iojbl.cn

Py:   isinstance(u, User)
来源：http://ekb.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://qen.bbcook.cn

JS:   u instanceof User
来源：http://sbw.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ktj.shuidangran.top

Java: u instanceof User
来源：http://lep.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://bwg.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://zpc.gzhubu.top

C#:   u is User
来源：http://juv.jianghu66.top

[G14] 数据类 / record
来源：http://ssb.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dns.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://wfg.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://yjp.sjlbkw.cn

TS:   type User = { name: string; age: number };
来源：http://pnq.birdmap.top

Java: record User(String name, int age) {}
来源：http://zxn.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://rxc.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xhf.ivvv.top

C#:   record User(string Name, int Age);
来源：http://pjy.jqgufenzy.top

[G15] 枚举
来源：http://usc.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bge.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ely.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mlc.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ysa.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://rcq.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gyj.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://ndi.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rgq.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://hnj.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qbu.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://lsc.yonumen.top

JS:   Object.entries(obj)
来源：http://spp.svipenyu.cn

TS:   Object.entries(obj)
来源：http://bja.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://btf.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yak.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://pnk.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://opl.sweek.top

================================================================================
来源：http://rez.cashguo.top

H. 异常与错误处理
来源：http://jjx.bbcook.cn

================================================================================
来源：http://llf.gzhubu.top

[H01] try / catch 基础
来源：http://rsu.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://irg.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bnm.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cmn.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rar.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://txv.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ipf.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rrv.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ovu.daria6918.cn

[H02] finally / ensure 收尾
来源：http://day.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://jtg.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://qdz.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://eco.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bsf.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://ome.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ngb.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://pev.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pwa.yongpay.top

[H03] 主动抛出异常
来源：http://rdk.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://wnu.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zqq.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://vub.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://kgf.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yyk.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bxt.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://vvb.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://kwq.zhixingplan.top

[H04] 自定义异常类型
来源：http://gup.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://wne.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://abw.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://xot.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://zcs.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://gcu.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cbw.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://btv.epnwcf.com

C#:   class MyException : Exception {}
来源：http://vlp.quarkkingdee.top

[H05] 捕获特定类型
来源：http://txn.jyoumei.cn

Py:   except ValueError as e:
来源：http://ryu.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cyl.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://sle.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://iti.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://xjg.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://odl.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://ndp.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dww.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://ukc.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://eso.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://omr.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://jsc.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://ifr.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://guu.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vcw.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://fdt.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://fgx.yongpay.top

[H07] 断言
来源：http://eak.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://ble.ivvv.top

PHP:  assert($x > 0);
来源：http://tou.hcnkem.com

JS:   console.assert(x > 0);
来源：http://lpi.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://isv.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://los.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bti.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://cnm.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://wcy.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://adm.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://gox.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fme.havefunace.top

JS:   e.message;  e.stack
来源：http://qwl.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jvl.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cuf.meibo888.top

Go:   err.Error()
来源：http://jdp.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://nin.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://okm.fengsongda.top

[H09] 带错误码的异常
来源：http://fzt.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ixn.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://jmb.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lcq.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://umn.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://edm.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rgi.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ygl.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xvi.shzxlz.cn

[H10] 资源自动释放
来源：http://ptn.xuanzx.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vfu.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://crd.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pik.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bzt.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://guo.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://erw.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://twy.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hfj.tian-w.cn

================================================================================
来源：http://pnt.hnxiangtu.top

I. 正则表达式
来源：http://rha.zhijiandao.cn

================================================================================
来源：http://rna.nanxuanxn.top

[I01] 判断是否匹配
来源：http://irl.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vcg.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lbt.yj20258.top

JS:   /\d+/.test(s)
来源：http://vza.guannengcc.top

TS:   /\d+/.test(s)
来源：http://ukq.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://olt.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gga.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://yfr.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rxa.shzxlz.cn

[I02] 提取所有匹配
来源：http://vxl.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://lyq.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fib.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mdk.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://lny.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gtt.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cfh.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://zud.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://frh.hcnkem.com

[I03] 提取捕获分组
来源：http://laq.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tif.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pmg.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hzj.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://okb.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kni.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tbv.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mro.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lwo.xuetiantiany.cn

[I04] 正则替换
来源：http://hvw.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rqd.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oxc.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://eqy.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://qru.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://zbw.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jpn.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://ktk.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pfg.zhengqikj.top

[I05] 按正则拆分
来源：http://yvd.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gby.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zyt.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://wtn.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://vir.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://qwt.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dlv.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://bdc.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lvd.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kyg.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wzg.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vlm.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bwt.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fue.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jsr.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blc.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://loo.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zsl.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://iyz.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nhn.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uqb.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ysx.ywan-chungtsiang.top

TS:   /error/gim
来源：http://zok.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vxw.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dzn.birdmap.top

Ruby: s.scan(/error/i)
来源：http://yss.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ivd.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://ibu.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tdd.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gcm.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tdh.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dml.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://rtl.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yws.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mvs.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lbp.zhijiandao.cn

================================================================================
来源：http://ehe.epnwcf.com

J. 日期与时间
来源：http://gja.yuanzhike.top

================================================================================
来源：http://lkg.nwbrower.top

[J01] 获取当前时间
来源：http://psj.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ygg.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ncy.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://ymk.snrcjt.cn

TS:   new Date();  Date.now()
来源：http://mex.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://thf.cheryme.top

Go:   time.Now()
来源：http://jdp.dashuyun.cn

Ruby: Time.now
来源：http://kcr.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wmy.shangyingyoupin.top

[J02] 格式化输出
来源：http://rls.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpi.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hdn.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jjl.yvedp.cn

TS:   d.toISOString()
来源：http://gwf.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wgv.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zbi.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwa.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tvc.hywenlv.cn

[J03] 字符串解析为日期
来源：http://tmr.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dsf.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pcd.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://zxo.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://wwd.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gyi.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rnj.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://iki.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ria.uphjek.com

[J04] 时间戳与日期互转
来源：http://ksc.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cxh.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vkd.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vii.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eqs.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hnm.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ssk.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tzg.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vcr.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://vwi.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://mlu.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kah.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ykz.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwf.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://qon.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gxj.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://pjg.sufxvd.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sqf.yj202588.top

[J06] 计算两时间之差
来源：http://zdm.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://eqq.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://umv.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sfm.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jqx.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://sfl.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://ern.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://kfm.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://qcl.sweek.top


<!-- 参考信息 -->