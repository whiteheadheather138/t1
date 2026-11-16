代发 wailian999

Java: interface Shape { double area(); }
来源：http://lfh.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://shs.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ffp.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://gwt.fzhhl.top

[G10] 访问控制
来源：http://ssx.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://upg.xuetiantiany.cn

PHP:  public / protected / private
来源：http://ukg.bbcook.cn

JS:   #private 字段；其余公开
来源：http://sog.epnwcf.com

TS:   public / protected / private
来源：http://bcg.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://wvi.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tlv.hongshengwenyu.top

Ruby: public / protected / private
来源：http://zet.sxryk.cn

C#:   public / protected / private / internal
来源：http://qzr.cqqwz.cn

[G11] getter / setter
来源：http://utp.fzhhl.top

Py:   @property 与 @x.setter
来源：http://cnb.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ekl.yvedp.cn

JS:   get name() { return this._name; }
来源：http://wah.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://nwv.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://kzy.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://xyj.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://mjr.bbcook.cn

C#:   public string Name { get; set; }
来源：http://rkb.zhijiandao.cn

[G12] 对象转字符串
来源：http://tss.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://yya.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ufu.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://ntt.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://bli.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://wyd.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://mxu.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://uvf.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://jcf.guannengcc.top

[G13] 判断对象类型
来源：http://osn.hfpthk.cn

Py:   isinstance(u, User)
来源：http://axc.tianlin.xyz

PHP:  $u instanceof User
来源：http://pxj.yongpay.top

JS:   u instanceof User
来源：http://ptt.redwolf501.top

TS:   u instanceof User
来源：http://dmo.chenlongwang.top

Java: u instanceof User
来源：http://oqx.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://adm.fengsongda.top

Ruby: u.is_a?(User)
来源：http://dct.hcnkem.com

C#:   u is User
来源：http://ovu.shangyingyoupin.top

[G14] 数据类 / record
来源：http://mqt.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qok.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://yxi.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://web.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://mow.sweek.top

Java: record User(String name, int age) {}
来源：http://ruh.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://myp.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cgy.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://lto.gzhubu.top

[G15] 枚举
来源：http://vlg.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fju.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ivo.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xtf.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eoa.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://gcq.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rbj.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://wea.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uxh.ivvv.top

[G16] 对象转数组 / 字典
来源：http://odd.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xbe.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://eti.hysaishi.cn

JS:   Object.entries(obj)
来源：http://dte.zhixingplan.top

TS:   Object.entries(obj)
来源：http://ngq.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kjk.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://htn.gotoacloud.top

Ruby: obj.instance_variables
来源：http://jxe.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://flm.jlsjyb.cn

================================================================================
来源：http://hsj.iojbl.cn

H. 异常与错误处理
来源：http://lmm.fzhhl.top

================================================================================
来源：http://eic.guowangkeji.top

[H01] try / catch 基础
来源：http://gjr.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oie.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qks.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ymp.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://upi.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pmd.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://omq.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xtd.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hog.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://wtv.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yjq.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lxs.jinyuanbaomall.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rzi.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pzd.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xlp.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbu.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://red.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fnn.hfpthk.cn

[H03] 主动抛出异常
来源：http://bjz.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://vkk.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://upy.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://tgs.tarul.cn

TS:   throw new Error("错误信息");
来源：http://upf.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://oet.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zas.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ymd.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://izp.quarkkingdee.top

[H04] 自定义异常类型
来源：http://enu.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://iui.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://vcg.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://zmv.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://sxr.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://rpi.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mis.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://enh.yueranfly.top

C#:   class MyException : Exception {}
来源：http://wdp.gotoacloud.top

[H05] 捕获特定类型
来源：http://dlu.aibaodan.cn

Py:   except ValueError as e:
来源：http://spu.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ouo.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://duv.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://xzi.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://fcb.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mly.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://nto.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iie.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://nyk.yongpay.top

Py:   value = d.get("k") or default
来源：http://efh.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://cac.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://rrg.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fju.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ihx.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hqo.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://teb.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://yld.yongpay.top

[H07] 断言
来源：http://iph.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://uif.yfazqb.com

PHP:  assert($x > 0);
来源：http://qoh.fengsongda.top

JS:   console.assert(x > 0);
来源：http://vbw.fengsongda.top

TS:   console.assert(x > 0);
来源：http://prv.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://rgf.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yxq.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rqf.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://ida.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://viw.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://hmx.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://heo.iojbl.cn

JS:   e.message;  e.stack
来源：http://mkn.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://caa.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jam.zdbjq.cn

Go:   err.Error()
来源：http://tru.sweek.top

Ruby: e.message;  e.backtrace
来源：http://tmp.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://sce.svipenyu.cn

[H09] 带错误码的异常
来源：http://dih.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://upv.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zit.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gvg.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dwq.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nqg.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nmm.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ycg.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rbr.ivvv.top

[H10] 资源自动释放
来源：http://beg.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dep.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uhk.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eer.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mtu.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://npr.yj20258.top

Go:   defer f.Close()
来源：http://wbb.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rrs.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://prm.daxiang520.top

================================================================================
来源：http://mhg.hnqzz.top

I. 正则表达式
来源：http://vcv.316326.xyz

================================================================================
来源：http://qcw.zhengqikj.top

[I01] 判断是否匹配
来源：http://hcv.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dis.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://ozy.sweek.top

JS:   /\d+/.test(s)
来源：http://xqv.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://rwd.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pzs.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rmk.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://umb.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jcv.chenlongwang.top

[I02] 提取所有匹配
来源：http://rby.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://upg.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xor.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ael.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://dpw.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qcz.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wsu.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://pbh.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cgw.smart0.xyz

[I03] 提取捕获分组
来源：http://que.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ggy.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lay.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rlu.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cqr.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lth.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ofh.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mpi.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hvo.nanxinkj.top

[I04] 正则替换
来源：http://hqj.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://gcn.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://szn.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://axy.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eft.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://nga.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wbc.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kvw.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wqu.zhiwuduotai.top

[I05] 按正则拆分
来源：http://ump.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sxb.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xiq.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://mqa.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://xkn.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://cpo.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qeq.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://klc.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qav.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hvy.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iye.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rpl.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmx.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vac.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bdy.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://inj.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qid.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ndi.sweek.top

[I07] 忽略大小写与多行模式
来源：http://rzv.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pby.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ffr.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uuq.ybcxt.top

TS:   /error/gim
来源：http://ilp.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qsn.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dhv.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://ihg.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lxy.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://fnw.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ydn.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wxd.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nzt.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ntp.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lpc.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vjc.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kci.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hji.zhaomingkeji.xyz

================================================================================
来源：http://qea.hnxiangtu.top

J. 日期与时间
来源：http://xdy.shanyushiyangkeji.top

================================================================================
来源：http://gug.pengpengdd.cyou

[J01] 获取当前时间
来源：http://mzj.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vqx.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jjh.cashguo.top

JS:   new Date();  Date.now()
来源：http://azi.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://cfr.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mhh.jianghu66.top

Go:   time.Now()
来源：http://hpv.sxryk.cn

Ruby: Time.now
来源：http://xtu.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nyg.yj20258888.top

[J02] 格式化输出
来源：http://paq.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tje.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nkb.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nlw.iojbl.cn

TS:   d.toISOString()
来源：http://kps.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://htb.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wpc.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovw.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://psp.mhx1999.top

[J03] 字符串解析为日期
来源：http://wdg.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yji.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ipw.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://wei.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://vra.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://msu.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jnl.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://bgy.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://arx.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://zrd.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://luv.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qfp.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ezv.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://enw.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xct.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ito.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qxv.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lzb.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://atn.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://kve.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://abj.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfn.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kcj.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://ihn.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bks.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://fea.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vdi.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://jrj.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://epl.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://mwo.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qms.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cer.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://hej.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://cjl.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://agq.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://toz.nwbrower.top

[J07] 比较两个日期
来源：http://ijs.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://oic.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oql.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aip.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hpz.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rms.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sqi.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wfc.jlsjyb.cn


<!-- 参考信息 -->