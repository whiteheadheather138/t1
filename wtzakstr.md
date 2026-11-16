代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wcm.jinqigufen.top

Ruby: def self.f; end
来源：http://zsd.dianchejie.cn

C#:   public static void F() {}
来源：http://std.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://bdk.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://oev.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yzp.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dox.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://klv.xinyue.icu

Java: interface Shape { double area(); }
来源：http://opp.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://hox.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hxi.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://kap.hnxiangtu.top

[G10] 访问控制
来源：http://xyc.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://ior.daxiang520.top

PHP:  public / protected / private
来源：http://bkh.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://wfi.mhx1999.top

TS:   public / protected / private
来源：http://jye.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://pcf.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://gfi.gaohongyu789.top

Ruby: public / protected / private
来源：http://tlg.hesvh.cn

C#:   public / protected / private / internal
来源：http://ebz.yfazqb.com

[G11] getter / setter
来源：http://zlq.yvedp.cn

Py:   @property 与 @x.setter
来源：http://krc.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cfp.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://qcu.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://qkx.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://mfg.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ptc.zhixingplan.top

Ruby: attr_accessor :name
来源：http://fof.yvedp.cn

C#:   public string Name { get; set; }
来源：http://ccu.jlsjyb.cn

[G12] 对象转字符串
来源：http://grl.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://lhs.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gdx.tarul.cn

JS:   toString() { return this.name; }
来源：http://msi.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://ono.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://lsg.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://ryx.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://mtt.tarul.cn

C#:   public override string ToString() => Name;
来源：http://xmb.zycfv.cn

[G13] 判断对象类型
来源：http://mue.zhengqikj.top

Py:   isinstance(u, User)
来源：http://typ.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://qyv.xinyue.icu

JS:   u instanceof User
来源：http://lpe.bbcook.cn

TS:   u instanceof User
来源：http://ctv.shuidangran.top

Java: u instanceof User
来源：http://ect.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://njq.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://yko.zhixingplan.top

C#:   u is User
来源：http://cqy.chenjidiqi.icu

[G14] 数据类 / record
来源：http://xgy.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mtc.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ifl.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://hpt.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://hig.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://pyk.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://bfn.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fzs.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://lxv.hnxiangtu.top

[G15] 枚举
来源：http://ooh.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fcd.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jat.c1oappe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rgh.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rtq.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://cdt.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hca.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://gcv.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yvt.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://gkp.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ypv.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://csv.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://cas.dianchejie.cn

TS:   Object.entries(obj)
来源：http://eya.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vjz.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rgw.yuanzhike.top

Ruby: obj.instance_variables
来源：http://sgp.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://gao.gzhubu.top

================================================================================
来源：http://qow.yongpay.top

H. 异常与错误处理
来源：http://wom.cqqwz.cn

================================================================================
来源：http://ajr.cashguo.top

[H01] try / catch 基础
来源：http://uup.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ajr.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://igc.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ugi.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wyz.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxc.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kmb.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kst.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vsf.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://zbq.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://aqj.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dxa.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cjp.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://xvu.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iid.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pvw.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yhu.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ykx.meibo888.top

[H03] 主动抛出异常
来源：http://epg.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://het.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://prb.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://upa.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://hof.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zet.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sey.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lbn.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://omx.shuidangran.top

[H04] 自定义异常类型
来源：http://cju.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://wrd.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://sae.yueranfly.top

JS:   class MyError extends Error {}
来源：http://aia.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://qct.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://bhm.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nyo.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://kdj.fktsv.cn

C#:   class MyException : Exception {}
来源：http://zvm.9152youxi.cn

[H05] 捕获特定类型
来源：http://iny.yanxiufei.cn

Py:   except ValueError as e:
来源：http://odq.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://akw.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://yug.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://qxx.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://cdd.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dyd.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://hew.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pox.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://jtz.sysykeji.top

Py:   value = d.get("k") or default
来源：http://ghl.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://wmx.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://pyq.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ykx.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ajl.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://evi.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://ake.meibo888.top

C#:   obj?.A?.B ?? default
来源：http://jkw.cashguo.top

[H07] 断言
来源：http://kst.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://wdk.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://orp.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://lxe.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://amp.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://cka.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://miy.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://yos.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://otk.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://rtk.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://uso.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qto.yfazqb.com

JS:   e.message;  e.stack
来源：http://wso.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bhk.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lem.yongpay.top

Go:   err.Error()
来源：http://usi.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://apl.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://svk.xinyue.icu

[H09] 带错误码的异常
来源：http://jge.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jml.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rad.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wvx.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dko.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vjf.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oqo.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qzf.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bbl.sweek.top

[H10] 资源自动释放
来源：http://dro.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rhz.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gyn.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqx.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bpj.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hzm.chenlongwang.top

Go:   defer f.Close()
来源：http://tvb.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fdk.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yau.wangdashe.top

================================================================================
来源：http://mpi.yongpay.top

I. 正则表达式
来源：http://ffw.316326.xyz

================================================================================
来源：http://mhw.ybcxt.top

[I01] 判断是否匹配
来源：http://ugb.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kwq.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://udm.sysykeji.top

JS:   /\d+/.test(s)
来源：http://rfb.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://frr.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://izs.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ijo.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://erp.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hvj.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://qxm.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://lqv.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://btm.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://elb.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://mhv.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ase.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wvi.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://udl.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zin.aibaodan.cn

[I03] 提取捕获分组
来源：http://kvs.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://adl.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sfz.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yil.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xrc.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vgf.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nfg.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://stj.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jrr.hesvh.cn

[I04] 正则替换
来源：http://cjv.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tiv.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbd.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ond.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tby.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ttr.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://qns.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pim.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uhb.jinqigfzy.top

[I05] 按正则拆分
来源：http://xmd.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sbb.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qon.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://rvb.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://qez.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://byi.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://flt.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fro.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ace.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://irq.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://snh.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zdu.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pxu.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbp.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nmn.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vpb.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://asv.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ebr.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://pza.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jce.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gxm.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hkt.hammf.cn

TS:   /error/gim
来源：http://sbs.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://spw.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xrk.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://lub.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://czt.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://hjl.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ejd.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nkh.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybx.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cay.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://roh.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zto.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ehm.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fpi.fengsongda.top

================================================================================
来源：http://ehc.gaohongyu789.top

J. 日期与时间
来源：http://lav.ydjk.org.cn

================================================================================
来源：http://xvu.dianchejie.cn

[J01] 获取当前时间
来源：http://hlu.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wmf.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dyj.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://uvr.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://jzj.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://juo.cqqwz.cn

Go:   time.Now()
来源：http://srh.sjlbkw.cn

Ruby: Time.now
来源：http://ato.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lgo.hesvh.cn

[J02] 格式化输出
来源：http://dxi.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mou.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aqm.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ulw.vqdsnc.cn

TS:   d.toISOString()
来源：http://lpw.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ffs.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://udj.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdj.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jlv.yongpay.top

[J03] 字符串解析为日期
来源：http://yld.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://upb.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gya.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://thp.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://juj.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wct.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://abb.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://avd.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://klo.ydzc1.top

[J04] 时间戳与日期互转
来源：http://zes.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jcv.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tbb.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ivb.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://fnl.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rhf.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wwn.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nxt.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yij.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://jpv.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://sye.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://sfi.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iev.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gmm.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://ett.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fum.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://scm.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zkp.cqqwz.cn

[J06] 计算两时间之差
来源：http://ndq.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://fec.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://kqg.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jox.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abd.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://gwo.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://zdd.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://ory.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://cjc.chenzaomai.com


<!-- 参考信息 -->