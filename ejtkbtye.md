代发 wailian999

JS:   super.greet();
来源：http://svj.ybcxt.top

TS:   super.greet();
来源：http://jmz.quarkkingdee.top

Java: super.greet();
来源：http://xec.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://luu.bbcook.cn

Ruby: super
来源：http://mvs.tanke756.top

C#:   base.Greet();
来源：http://fdp.iojbl.cn

[G08] 静态方法与属性
来源：http://gvf.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbs.ydzc1.top

PHP:  public static function f() {}
来源：http://iii.yonumen.top

JS:   static f() {}
来源：http://qtz.xziqi.cn

TS:   static f(): void {}
来源：http://rpe.yongpay.top

Java: static void f() {}
来源：http://qdw.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://trb.sufxvd.cn

Ruby: def self.f; end
来源：http://tpp.quarkkingdee.top

C#:   public static void F() {}
来源：http://pzc.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://wec.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://kmv.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://kjr.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ofn.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://fwi.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://lmf.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://kml.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rsq.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://kpp.uphjek.com

[G10] 访问控制
来源：http://bvt.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://iwo.fzhhl.top

PHP:  public / protected / private
来源：http://luv.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://puy.yj202588.top

TS:   public / protected / private
来源：http://vdc.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://ywn.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pnm.hcnkem.com

Ruby: public / protected / private
来源：http://lcf.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://mfo.ppjwa.cn

[G11] getter / setter
来源：http://meb.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://vrp.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://sca.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://phf.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://vog.sweek.top

Java: public String getName() { return name; }
来源：http://ryx.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://ohy.tarul.cn

Ruby: attr_accessor :name
来源：http://cin.xylfe.cn

C#:   public string Name { get; set; }
来源：http://opr.ydjk.org.cn

[G12] 对象转字符串
来源：http://ysx.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://idj.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mdx.havefunace.top

JS:   toString() { return this.name; }
来源：http://zxx.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://yim.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://wue.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://rmo.birdmap.top

Ruby: def to_s; @name; end
来源：http://zpp.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://epj.vqdsnc.cn

[G13] 判断对象类型
来源：http://kgr.fktsv.cn

Py:   isinstance(u, User)
来源：http://cfh.hysaishi.cn

PHP:  $u instanceof User
来源：http://ssu.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://izs.nwbrower.top

TS:   u instanceof User
来源：http://eky.ppjwa.cn

Java: u instanceof User
来源：http://rmb.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ukw.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://mmo.yonumen.top

C#:   u is User
来源：http://wly.sjlbkw.cn

[G14] 数据类 / record
来源：http://bng.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wee.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://iwg.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://xos.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://irf.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://gnq.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://ayj.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xpv.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://iiv.ywan-chungtsiang.top

[G15] 枚举
来源：http://fey.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ypd.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufu.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vmt.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pxs.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://lcm.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://upe.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://mli.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sag.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://lrq.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://elf.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://xxi.hesvh.cn

JS:   Object.entries(obj)
来源：http://bmw.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://che.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qjv.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://gpg.yj202588.top

Ruby: obj.instance_variables
来源：http://vwb.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://lzr.haohaochexian.top

================================================================================
来源：http://trk.gogol.net.cn

H. 异常与错误处理
来源：http://yfp.hesvh.cn

================================================================================
来源：http://nzy.xinyue.icu

[H01] try / catch 基础
来源：http://sgm.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://egd.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://stx.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lnm.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://okq.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nzq.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ckg.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vjr.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mko.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://qsg.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://vri.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uin.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://prz.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uxf.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://sbl.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fwu.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://qzp.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://miu.uphjek.com

[H03] 主动抛出异常
来源：http://jrd.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://qrw.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qmy.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://dgl.uphjek.com

TS:   throw new Error("错误信息");
来源：http://ute.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rfz.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pyu.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jai.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nlw.shuidangran.top

[H04] 自定义异常类型
来源：http://isj.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://fue.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://lhb.gzhubu.top

JS:   class MyError extends Error {}
来源：http://rrl.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://oau.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://gic.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://apj.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://xmz.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://cmf.zycfv.cn

[H05] 捕获特定类型
来源：http://vat.nanxuanxn.top

Py:   except ValueError as e:
来源：http://jhw.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xof.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://upb.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://bwr.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://wxz.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dej.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://ixy.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hoa.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://gxb.andypj.xyz

Py:   value = d.get("k") or default
来源：http://sud.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://web.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://eul.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rhe.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://exw.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xgu.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://nck.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://qmg.ehwqpu.com

[H07] 断言
来源：http://jca.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://oas.cashguo.top

PHP:  assert($x > 0);
来源：http://pha.xziqi.cn

JS:   console.assert(x > 0);
来源：http://qlx.bbcook.cn

TS:   console.assert(x > 0);
来源：http://qbt.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://bxy.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://frp.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://vwf.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://xmj.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://qql.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://lqz.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://weu.sufxvd.cn

JS:   e.message;  e.stack
来源：http://xvc.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pnh.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://etu.zhaomingkeji.xyz

Go:   err.Error()
来源：http://kah.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://ony.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://iru.haohaochexian.top

[H09] 带错误码的异常
来源：http://ieb.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://caw.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wph.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cos.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ums.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://syc.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iyp.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://knd.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vmy.316326.xyz

[H10] 资源自动释放
来源：http://vlw.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://miy.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lfr.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tzk.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dvw.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwq.zhengqikj.top

Go:   defer f.Close()
来源：http://qgh.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wep.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mwu.tianlin.xyz

================================================================================
来源：http://ayx.shanyushiyangtech.top

I. 正则表达式
来源：http://kuu.zdqjudy.top

================================================================================
来源：http://jev.cdnleiting.top

[I01] 判断是否匹配
来源：http://wzf.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://azn.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://nut.mhx1999.top

JS:   /\d+/.test(s)
来源：http://xst.bjfxy.top

TS:   /\d+/.test(s)
来源：http://fvz.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tpr.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wua.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://qlf.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kcs.tarul.cn

[I02] 提取所有匹配
来源：http://huc.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://yzh.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tom.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gqt.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://ovr.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fdk.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ikj.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://pdg.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zis.tian-w.cn

[I03] 提取捕获分组
来源：http://qaa.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mvi.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rfv.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dio.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sbi.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ulp.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fpn.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rsn.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iri.andypj.xyz

[I04] 正则替换
来源：http://fnr.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://djd.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pwe.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://brp.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jrp.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://ebg.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xut.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tqj.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://com.dianchejie.cn

[I05] 按正则拆分
来源：http://yas.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nci.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gdn.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://nvd.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://bqf.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://lwc.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fgz.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vzy.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tie.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bns.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xlo.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dgl.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pft.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tnn.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://taf.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gol.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pyt.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://okh.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://yhb.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jva.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://frn.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tza.sufxvd.cn

TS:   /error/gim
来源：http://rfe.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bmt.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hcc.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://qen.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cdc.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://qnn.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mic.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kfe.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjc.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lps.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://jml.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ssb.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zdp.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vdv.zdbjq.cn

================================================================================
来源：http://mwe.fehbvm.com

J. 日期与时间
来源：http://eox.aibaodan.cn

================================================================================
来源：http://vvv.fengsongda.top

[J01] 获取当前时间
来源：http://chn.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ksv.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xgv.bbcook.cn

JS:   new Date();  Date.now()
来源：http://ymj.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://bho.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://vte.jqgfzy.top

Go:   time.Now()
来源：http://oyu.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://yzt.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ndt.guowangkeji.top

[J02] 格式化输出
来源：http://zkh.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bmk.pycfn.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lek.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nwm.shangyingyoupin.top

TS:   d.toISOString()
来源：http://xbh.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fdi.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://igg.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qxg.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://plg.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://ret.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gfq.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eye.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://feo.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://cwg.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://yla.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hnq.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://pyv.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bue.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://vsj.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://owx.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vfc.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tyj.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yra.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hzn.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jta.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tij.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xxl.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://rva.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://xoa.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xze.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hlh.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzy.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://lhk.aizwys.cn


<!-- 参考信息 -->