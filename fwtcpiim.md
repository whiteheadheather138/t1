代发 wailian999

Java: interface Shape { double area(); }
来源：http://bru.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://fjn.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zwg.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://zlq.hysaishi.cn

[G10] 访问控制
来源：http://wyk.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://mxr.ppjwa.cn

PHP:  public / protected / private
来源：http://sci.sweek.top

JS:   #private 字段；其余公开
来源：http://wli.bjfxy.top

TS:   public / protected / private
来源：http://vfe.meibo888.top

Java: public / protected / private / 默认包级
来源：http://jvu.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://egw.yj202588.top

Ruby: public / protected / private
来源：http://gkv.aibaodan.cn

C#:   public / protected / private / internal
来源：http://qmm.0kj1m.cn

[G11] getter / setter
来源：http://fmd.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://xzc.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tje.redwolf501.top

JS:   get name() { return this._name; }
来源：http://vvj.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://xba.uphjek.com

Java: public String getName() { return name; }
来源：http://ssb.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://sss.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://jtb.fktsv.cn

C#:   public string Name { get; set; }
来源：http://iqt.pycfn.com

[G12] 对象转字符串
来源：http://jda.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://gxx.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://guq.yongpay.top

JS:   toString() { return this.name; }
来源：http://tpl.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://ehy.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://aug.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://jdt.tian-w.cn

Ruby: def to_s; @name; end
来源：http://otf.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://izz.316326.xyz

[G13] 判断对象类型
来源：http://jle.316326.xyz

Py:   isinstance(u, User)
来源：http://the.jinqigfzy.top

PHP:  $u instanceof User
来源：http://ckg.hongshengwenyu.top

JS:   u instanceof User
来源：http://nzf.guannengcc.top

TS:   u instanceof User
来源：http://now.daria6918.cn

Java: u instanceof User
来源：http://scx.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gjy.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://fvh.hnqzz.top

C#:   u is User
来源：http://ywv.dianchejie.cn

[G14] 数据类 / record
来源：http://uuo.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ksr.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://gyh.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wdp.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://ldd.xylfe.cn

Java: record User(String name, int age) {}
来源：http://rwf.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://hpb.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://isc.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://wfw.haohaochexian.top

[G15] 枚举
来源：http://mpk.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fya.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vgs.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oke.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xzv.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://cra.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ump.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://sgh.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://btf.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://csj.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cxq.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://drk.bjfxy.top

JS:   Object.entries(obj)
来源：http://glj.cqqwz.cn

TS:   Object.entries(obj)
来源：http://kgv.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ayg.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zzb.c1oappe.top

Ruby: obj.instance_variables
来源：http://nvy.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://pxd.cucudq.cn

================================================================================
来源：http://hub.yangfankeji.com

H. 异常与错误处理
来源：http://bln.nanxinkj.top

================================================================================
来源：http://efi.xinyue.icu

[H01] try / catch 基础
来源：http://chk.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gzg.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fzv.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nwh.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ujw.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ghy.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xeg.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yaw.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lrz.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://lui.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://vhu.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nzd.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dyy.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://emo.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://tcu.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iws.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dhq.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://otd.yanxiufei.cn

[H03] 主动抛出异常
来源：http://qcp.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://tvi.epnwcf.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://quv.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://kkp.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://uih.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wly.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gjk.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hdx.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kaa.guowangkeji.top

[H04] 自定义异常类型
来源：http://rgp.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://plq.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://pvm.xylfe.cn

JS:   class MyError extends Error {}
来源：http://kjb.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://oph.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://zms.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qvd.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://jwh.fzhhl.top

C#:   class MyException : Exception {}
来源：http://fep.cqqwz.cn

[H05] 捕获特定类型
来源：http://muf.yj20258888.top

Py:   except ValueError as e:
来源：http://rxl.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wgh.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://ttx.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://rkk.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://wfr.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://omd.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://ohv.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sge.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://fyr.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://tbb.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wez.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://ooq.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://nmx.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ool.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://hlo.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://hiq.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://ato.jiagoushi.top

[H07] 断言
来源：http://vwm.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://ert.zdbjq.cn

PHP:  assert($x > 0);
来源：http://uxk.yuxming.cn

JS:   console.assert(x > 0);
来源：http://uog.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://emq.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://iiz.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ume.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://zan.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://lpu.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://zac.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://ltr.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://grq.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://wnn.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ida.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vvq.fehbvm.com

Go:   err.Error()
来源：http://zeu.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://tan.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://hat.guowangkeji.top

[H09] 带错误码的异常
来源：http://gqt.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpi.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://qwp.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qna.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iuv.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rmd.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bak.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://xcw.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dja.guannengcc.top

[H10] 资源自动释放
来源：http://pap.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dki.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dlg.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cio.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ivr.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pwg.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://vyp.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://exr.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lim.yfazqb.com

================================================================================
来源：http://iwz.ywan-chungtsiang.top

I. 正则表达式
来源：http://ofg.hfpthk.cn

================================================================================
来源：http://mzl.jqgfzy.top

[I01] 判断是否匹配
来源：http://skz.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://miq.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://wwn.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://amp.vehdjk.com

TS:   /\d+/.test(s)
来源：http://xxv.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aex.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hxa.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://jox.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://apb.c1oappe.top

[I02] 提取所有匹配
来源：http://lcb.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://scj.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kxj.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rub.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://kyp.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hpd.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://anx.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://iuj.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gqr.jiagoushi.top

[I03] 提取捕获分组
来源：http://blf.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://njb.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ycv.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qam.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://czt.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://usg.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://csh.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wcl.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oon.mhx1999.top

[I04] 正则替换
来源：http://jkx.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zva.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://arw.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cyd.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://phs.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nin.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rjd.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iwn.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zjm.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://xtu.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://yfr.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ayf.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://hsv.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://qqa.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://qdz.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yxc.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://eig.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zxe.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hcl.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iaa.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://obl.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxp.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aos.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bil.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yco.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kjk.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hik.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://ncy.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fqv.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tel.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gtn.0kj1m.cn

TS:   /error/gim
来源：http://gjg.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aul.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tvy.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://muj.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jtu.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://jse.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qhm.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wma.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tnp.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://edi.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ddr.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ffv.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bvt.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://exb.0kj1m.cn

================================================================================
来源：http://aff.pycfn.com

J. 日期与时间
来源：http://xgz.jlsjyb.cn

================================================================================
来源：http://nuh.tarul.cn

[J01] 获取当前时间
来源：http://znw.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://erz.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pxq.vehdjk.com

JS:   new Date();  Date.now()
来源：http://krd.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://zlu.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://mbv.mhx1999.top

Go:   time.Now()
来源：http://gjh.daxiang520.top

Ruby: Time.now
来源：http://zjb.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wzw.tianlin.xyz

[J02] 格式化输出
来源：http://uma.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xdr.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://clr.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sbo.gogol.net.cn

TS:   d.toISOString()
来源：http://fog.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://reo.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jqm.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nyc.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gsj.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://zqk.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sir.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://izq.316326.xyz

JS:   new Date("2024-01-02")
来源：http://anq.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://mhc.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ure.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tfk.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://cyo.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lgw.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://qxn.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gwu.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zph.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qat.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vjy.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kmd.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vws.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gfv.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kms.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://lcr.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://aky.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lnn.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ryh.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kmn.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://nxh.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mwz.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://ddo.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sqi.wangdashe.top

[J06] 计算两时间之差
来源：http://cim.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://mlj.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://pte.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gbd.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfl.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qey.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://vpl.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://vga.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://uiv.haohaochexian.top

[J07] 比较两个日期
来源：http://bqr.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://lil.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rfw.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mwk.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://rcy.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://snj.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zzy.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vlq.feifeiyinyue.top


<!-- 参考信息 -->