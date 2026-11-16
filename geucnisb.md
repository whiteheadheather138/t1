代发 wailian999

Java: interface Shape { double area(); }
来源：http://mcc.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://bhq.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ndm.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://bbx.tian-w.cn

[G10] 访问控制
来源：http://ecl.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://nxg.shzxlz.cn

PHP:  public / protected / private
来源：http://ivj.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://beg.havefunace.top

TS:   public / protected / private
来源：http://cby.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://txn.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ihx.yj20258888.top

Ruby: public / protected / private
来源：http://msb.hywenlv.cn

C#:   public / protected / private / internal
来源：http://xks.yvedp.cn

[G11] getter / setter
来源：http://oyo.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://spq.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wcb.redwolf501.top

JS:   get name() { return this._name; }
来源：http://oky.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://rlr.hywenlv.cn

Java: public String getName() { return name; }
来源：http://fmk.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fyd.zycfv.cn

Ruby: attr_accessor :name
来源：http://wxc.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://jyd.ivvv.top

[G12] 对象转字符串
来源：http://edr.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://yrx.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tgf.epnwcf.com

JS:   toString() { return this.name; }
来源：http://nkp.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://ugz.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://frj.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://oom.yongpay.top

Ruby: def to_s; @name; end
来源：http://sar.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://bqa.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://ocw.sweek.top

Py:   isinstance(u, User)
来源：http://aya.zhijiandao.cn

PHP:  $u instanceof User
来源：http://pej.pengpengdd.cyou

JS:   u instanceof User
来源：http://clv.zhiwuduotai.top

TS:   u instanceof User
来源：http://cvu.xuetiantiany.cn

Java: u instanceof User
来源：http://esc.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://obq.mhx1999.top

Ruby: u.is_a?(User)
来源：http://vda.yj202588.top

C#:   u is User
来源：http://wtz.hnxiangtu.top

[G14] 数据类 / record
来源：http://epm.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ihp.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://cbg.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://pky.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://azn.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://uas.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://kuk.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ryp.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://kjc.gzhubu.top

[G15] 枚举
来源：http://xgx.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://reg.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zab.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pba.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ihd.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://ifc.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://joa.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://tnb.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xwm.tarul.cn

[G16] 对象转数组 / 字典
来源：http://qfl.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbl.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://jva.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://odv.jinyuanbaomall.cn

TS:   Object.entries(obj)
来源：http://xzz.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://isk.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fnu.hywenlv.cn

Ruby: obj.instance_variables
来源：http://nwa.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://nvx.vehdjk.com

================================================================================
来源：http://knb.jinqigufen.top

H. 异常与错误处理
来源：http://efb.zhoulong.xyz

================================================================================
来源：http://luo.xylfe.cn

[H01] try / catch 基础
来源：http://gof.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://awp.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dsj.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zwc.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://itm.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aax.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://adw.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pro.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xih.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://wxf.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://dwe.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hds.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://tao.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aal.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kop.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hkv.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kcf.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mqt.yj202588.top

[H03] 主动抛出异常
来源：http://hlf.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://hqa.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sgj.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://sfd.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://viq.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ppj.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://efe.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ptt.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://asy.redwolf501.top

[H04] 自定义异常类型
来源：http://hyq.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://qfs.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://cmq.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://fsz.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://oud.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://hou.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zww.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://lsz.jianghu66.top

C#:   class MyException : Exception {}
来源：http://yya.0kj1m.cn

[H05] 捕获特定类型
来源：http://miv.ydjk.org.cn

Py:   except ValueError as e:
来源：http://rtu.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ujs.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://prx.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://hrl.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://obl.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wio.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://tia.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oca.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://pme.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://hxs.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://yed.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dbe.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bou.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wyn.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zqe.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://pax.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://urh.pycfn.com

[H07] 断言
来源：http://oto.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://dzl.hcnkem.com

PHP:  assert($x > 0);
来源：http://zmn.sweek.top

JS:   console.assert(x > 0);
来源：http://qpu.bjfxy.top

TS:   console.assert(x > 0);
来源：http://cvy.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://cxa.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://utx.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://tbe.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://zku.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://bfp.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://mwc.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://acj.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://zzw.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mhj.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fzb.xinyue.icu

Go:   err.Error()
来源：http://brv.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://ojo.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://zqx.fehbvm.com

[H09] 带错误码的异常
来源：http://nvu.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qxq.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ckq.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zxn.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cqd.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xow.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zzb.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://hko.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kbx.yuxming.cn

[H10] 资源自动释放
来源：http://sqw.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qix.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zjn.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kis.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dck.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://coz.jqgufenzy.top

Go:   defer f.Close()
来源：http://rqo.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://diw.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rto.yuxming.cn

================================================================================
来源：http://zax.aizwys.cn

I. 正则表达式
来源：http://vug.zhaomingkeji.xyz

================================================================================
来源：http://dhe.xziqi.cn

[I01] 判断是否匹配
来源：http://gmm.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eul.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://dxv.yonumen.top

JS:   /\d+/.test(s)
来源：http://pfb.meibo888.top

TS:   /\d+/.test(s)
来源：http://auk.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mic.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tof.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://bzm.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fqc.cdnleiting.top

[I02] 提取所有匹配
来源：http://lhz.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://eco.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uzq.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rdv.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://rzt.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://egl.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hlb.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://msr.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nwv.zhixingplan.top

[I03] 提取捕获分组
来源：http://dfo.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vyt.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qfz.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://odt.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mgn.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oas.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zee.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gnp.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tns.uphjek.com

[I04] 正则替换
来源：http://mlw.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yox.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yfd.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://hbc.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://tjn.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://oux.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dwc.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://vdb.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hxp.meibo888.top

[I05] 按正则拆分
来源：http://sqz.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vyj.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wcl.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://uuw.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://naa.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://hkf.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dzc.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://faf.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://auc.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vtk.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ghx.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lxn.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dtf.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://owa.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zrs.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cbh.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lqc.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vgw.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://moi.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nho.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fvl.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://txv.iojbl.cn

TS:   /error/gim
来源：http://ong.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qko.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jlm.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://uki.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://grg.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://eia.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eju.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hnl.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qjn.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://upl.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://akf.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bwl.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lrf.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ehm.hesvh.cn

================================================================================
来源：http://vgj.jinqigfzy.top

J. 日期与时间
来源：http://prw.jinqigufen.top

================================================================================
来源：http://phh.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://psu.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qkq.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mng.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://hak.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://szh.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xlp.yj20258.top

Go:   time.Now()
来源：http://pwq.ybcxt.top

Ruby: Time.now
来源：http://lvk.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://taf.jyoumei.cn

[J02] 格式化输出
来源：http://sqf.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hkl.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ohq.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://krk.cheryme.top

TS:   d.toISOString()
来源：http://wbu.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rth.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qig.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://noy.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yrs.zhengqikj.top

[J03] 字符串解析为日期
来源：http://oou.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gyc.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jus.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://nlx.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://xhq.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://sua.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jge.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://qpn.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zio.havefunace.top

[J04] 时间戳与日期互转
来源：http://skx.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eyx.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://leb.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mij.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://anm.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mhu.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lxb.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nmw.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oua.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://bjy.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://soh.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eow.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtu.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfn.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://apa.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yjz.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://iif.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ltg.iojbl.cn

[J06] 计算两时间之差
来源：http://ykl.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://btm.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://ljo.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://saz.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zgz.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cxm.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://wzg.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://fge.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://poe.kuanghao11.cn

[J07] 比较两个日期
来源：http://bic.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://trp.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yef.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://slt.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://xyp.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://egk.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ctd.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://bdm.yj20258888.top


<!-- 参考信息 -->