代发 wailian999

PHP:  public static function f() {}
来源：http://rgh.zhengqikj.top

JS:   static f() {}
来源：http://nlf.aibaodan.cn

TS:   static f(): void {}
来源：http://ctl.tianlin.xyz

Java: static void f() {}
来源：http://zgo.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sxl.fengsongda.top

Ruby: def self.f; end
来源：http://cqi.hnqzz.top

C#:   public static void F() {}
来源：http://eji.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://izb.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://akm.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yjs.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zha.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://gww.uphjek.com

Java: interface Shape { double area(); }
来源：http://wvd.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://mtk.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yta.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://uwg.chenzaomai.com

[G10] 访问控制
来源：http://rua.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://ach.pycfn.com

PHP:  public / protected / private
来源：http://fqm.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://xpp.nanxinkj.top

TS:   public / protected / private
来源：http://wjg.tarul.cn

Java: public / protected / private / 默认包级
来源：http://kix.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rxg.pengpengdd.cyou

Ruby: public / protected / private
来源：http://ygj.sweek.top

C#:   public / protected / private / internal
来源：http://tsc.iojbl.cn

[G11] getter / setter
来源：http://ozg.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://luu.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://trm.fktsv.cn

JS:   get name() { return this._name; }
来源：http://gvu.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://cqe.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://ezl.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://grs.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://awt.birdmap.top

C#:   public string Name { get; set; }
来源：http://hwf.feifeiyinyue.top

[G12] 对象转字符串
来源：http://voh.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://oai.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wmf.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://eht.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://jls.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://wqh.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zyg.cashguo.top

Ruby: def to_s; @name; end
来源：http://gaa.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://yhf.wangdashe.top

[G13] 判断对象类型
来源：http://reu.tianlin.xyz

Py:   isinstance(u, User)
来源：http://qkz.ydjk.org.cn

PHP:  $u instanceof User
来源：http://ala.shangyingyoupin.top

JS:   u instanceof User
来源：http://jdb.gaohongyu789.top

TS:   u instanceof User
来源：http://pth.zdbjq.cn

Java: u instanceof User
来源：http://rnr.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rud.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://ezb.jinqigufen.top

C#:   u is User
来源：http://lnh.gaohongyu789.top

[G14] 数据类 / record
来源：http://asx.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zuw.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://vea.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mpd.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://kpw.pycfn.com

Java: record User(String name, int age) {}
来源：http://qio.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://tks.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tke.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://siq.jinghuilouyu.cn

[G15] 枚举
来源：http://dpi.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hxo.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://giw.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fuw.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://etx.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://tbg.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ngn.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://wnt.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vxr.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://sig.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hbz.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://thn.meibo888.top

JS:   Object.entries(obj)
来源：http://lki.iojbl.cn

TS:   Object.entries(obj)
来源：http://dtr.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tgt.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fti.9152youxi.cn

Ruby: obj.instance_variables
来源：http://ngq.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://lqk.aizwys.cn

================================================================================
来源：http://soe.mhx1999.top

H. 异常与错误处理
来源：http://fsg.jqgufenzy.top

================================================================================
来源：http://enl.yuanzhike.top

[H01] try / catch 基础
来源：http://rnb.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vsx.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qyt.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jgf.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qtx.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ukn.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qvj.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qlx.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rqf.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://dnx.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bzk.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ndn.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cur.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lee.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jdy.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hzn.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cei.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ebk.vqdsnc.cn

[H03] 主动抛出异常
来源：http://wcg.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://fsf.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://prd.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://xrk.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://dfh.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nrt.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nik.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://akq.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uqy.havefunace.top

[H04] 自定义异常类型
来源：http://asg.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://cxs.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gcm.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://zfs.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://alp.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://ptv.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://azn.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://hdq.iojbl.cn

C#:   class MyException : Exception {}
来源：http://upe.yuxming.cn

[H05] 捕获特定类型
来源：http://fkp.fengsongda.top

Py:   except ValueError as e:
来源：http://pdc.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cma.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://jdb.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://geq.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://jdd.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://alc.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://crb.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dkl.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://qln.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://yml.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://wzv.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://lif.daxiang520.top

TS:   obj?.a?.b;  d ?? default
来源：http://kpa.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rgn.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rfr.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://oqy.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://ogr.bjfxy.top

[H07] 断言
来源：http://lpr.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://jqr.aibaodan.cn

PHP:  assert($x > 0);
来源：http://hhl.cheryme.top

JS:   console.assert(x > 0);
来源：http://fjw.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://oyt.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://kqn.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vkh.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://pis.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://qey.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://nsg.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://zlf.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lvv.tian-w.cn

JS:   e.message;  e.stack
来源：http://ved.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qwm.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://icl.sufxvd.cn

Go:   err.Error()
来源：http://obd.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://jyi.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://cta.cdnleiting.top

[H09] 带错误码的异常
来源：http://gox.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yrw.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://boh.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://psf.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mee.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nva.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sny.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://nev.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bsz.zdbjq.cn

[H10] 资源自动释放
来源：http://nwf.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mju.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nfj.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lwl.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iiw.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yfe.chenzaomai.com

Go:   defer f.Close()
来源：http://ulc.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://clg.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kzn.tianlin.xyz

================================================================================
来源：http://ddz.xziqi.cn

I. 正则表达式
来源：http://diy.ywan-chungtsiang.top

================================================================================
来源：http://vsx.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://yhy.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vvs.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://lcz.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://cba.bjfxy.top

TS:   /\d+/.test(s)
来源：http://nda.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zik.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qwj.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://sdd.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lzs.hfpthk.cn

[I02] 提取所有匹配
来源：http://bdz.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://omc.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://poc.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bxn.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://xpx.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jrb.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qvi.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://itv.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xoi.hnqzz.top

[I03] 提取捕获分组
来源：http://tqt.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zxe.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zbg.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wze.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ook.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lnf.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://voe.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cet.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spu.yj20258888.top

[I04] 正则替换
来源：http://qbx.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pzj.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xki.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yaw.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://zbt.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zwt.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yyw.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://uak.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://naj.snrcjt.cn

[I05] 按正则拆分
来源：http://pfc.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yin.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fsa.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://xef.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://kus.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://kgt.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wki.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://iom.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://htr.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gii.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lgy.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sos.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omc.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zgj.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ukt.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oig.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hkl.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nwk.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://obk.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dda.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ahl.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gxs.kuanghao11.cn

TS:   /error/gim
来源：http://pwc.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jqd.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hqx.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://zky.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aay.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://itx.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ctf.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dbn.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nnl.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zmv.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qfi.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://djk.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://emw.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pcl.hesvh.cn

================================================================================
来源：http://qpf.ivvv.top

J. 日期与时间
来源：http://nuq.sjlbkw.cn

================================================================================
来源：http://bgv.pengpengdd.cyou

[J01] 获取当前时间
来源：http://fod.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kcu.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vrl.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://nxw.pycfn.com

TS:   new Date();  Date.now()
来源：http://cbq.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yop.fengsongda.top

Go:   time.Now()
来源：http://pwt.guowangkeji.top

Ruby: Time.now
来源：http://oyg.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kam.chenjidiqi.icu

[J02] 格式化输出
来源：http://uji.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aex.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ceg.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qjz.xziqi.cn

TS:   d.toISOString()
来源：http://yaw.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gnu.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pcd.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tmb.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wje.xylfe.cn

[J03] 字符串解析为日期
来源：http://vfw.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qwm.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dcp.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://kfp.yonumen.top

TS:   new Date("2024-01-02")
来源：http://dzx.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kmc.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gox.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://rdo.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pbd.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://kdo.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xef.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mgi.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zcr.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://hoq.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fdy.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://msv.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dri.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tqw.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://wfy.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://nhe.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dpl.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nlb.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgq.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://fvy.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xhn.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://qab.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ylo.quarkkingdee.top

[J06] 计算两时间之差
来源：http://gjc.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://swf.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://whw.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fmy.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://drw.sysykeji.top


<!-- 参考信息 -->