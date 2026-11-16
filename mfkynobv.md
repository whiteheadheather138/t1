代发 wailian999

C#:   public / protected / private / internal
来源：http://igo.zhengqikj.top

[G11] getter / setter
来源：http://zsx.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://hkm.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bde.uphjek.com

JS:   get name() { return this._name; }
来源：http://rea.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://wgl.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://jmm.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vgt.mhx1999.top

Ruby: attr_accessor :name
来源：http://sml.sweek.top

C#:   public string Name { get; set; }
来源：http://ufl.ctjpmb.com

[G12] 对象转字符串
来源：http://ult.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://uax.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wzv.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://pjc.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://edd.sweek.top

Java: @Override public String toString() { return name; }
来源：http://knp.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://akw.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://ccb.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://gzd.gotoacloud.top

[G13] 判断对象类型
来源：http://tum.fengsongda.top

Py:   isinstance(u, User)
来源：http://dwn.yuxming.cn

PHP:  $u instanceof User
来源：http://vdv.52xcode.cn

JS:   u instanceof User
来源：http://ysi.wangshuangyany.cn

TS:   u instanceof User
来源：http://cqp.hfpthk.cn

Java: u instanceof User
来源：http://qus.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aru.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://tpg.tanke756.top

C#:   u is User
来源：http://wny.c1oappe.top

[G14] 数据类 / record
来源：http://prv.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dcs.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://wxg.ivvv.top

JS:   // 无内置：普通类或对象字面量
来源：http://msd.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://ebn.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://ybk.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://lzx.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ypv.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://sty.yj202588.top

[G15] 枚举
来源：http://rha.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wsj.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://igi.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ntv.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ybf.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://fkh.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bxk.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://tep.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lmk.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://lnx.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fwj.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://znj.yonumen.top

JS:   Object.entries(obj)
来源：http://xnm.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://bjy.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sgo.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://qqo.snrcjt.cn

Ruby: obj.instance_variables
来源：http://nus.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://gkr.aibaodan.cn

================================================================================
来源：http://evi.birdmap.top

H. 异常与错误处理
来源：http://dcd.hammf.cn

================================================================================
来源：http://itx.hongshengwenyu.top

[H01] try / catch 基础
来源：http://dcq.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iwd.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://chv.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jds.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://itx.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gvn.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfo.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kgo.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nfm.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://zlx.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://yir.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hey.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gsv.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ixn.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://cwn.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://udo.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mss.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jfs.cashguo.top

[H03] 主动抛出异常
来源：http://gur.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://jat.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dnl.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://owp.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://ieh.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sre.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nkz.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mry.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://gtf.hcnkem.com

[H04] 自定义异常类型
来源：http://bmn.cashguo.top

Py:   class MyError(Exception): pass
来源：http://uxl.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tzh.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://rwk.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://mjx.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://bca.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zby.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://gsy.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://tyw.gzhubu.top

[H05] 捕获特定类型
来源：http://kiz.zhengqikj.top

Py:   except ValueError as e:
来源：http://vpa.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://htx.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://vcf.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://ruj.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://vtt.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jkc.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://ddb.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://doi.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://gpa.hnqzz.top

Py:   value = d.get("k") or default
来源：http://mca.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://ohc.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://jll.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://xhr.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fdj.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cks.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://tlc.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://ybl.yanxiufei.cn

[H07] 断言
来源：http://qtr.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://kai.dashuyun.cn

PHP:  assert($x > 0);
来源：http://npj.meibo888.top

JS:   console.assert(x > 0);
来源：http://ukj.shuidangran.top

TS:   console.assert(x > 0);
来源：http://prf.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://bpm.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mjb.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yid.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://uqt.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://atz.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://aah.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pni.cashguo.top

JS:   e.message;  e.stack
来源：http://sid.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kan.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nwa.jinqigufen.top

Go:   err.Error()
来源：http://eip.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://usy.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://idq.aibaodan.cn

[H09] 带错误码的异常
来源：http://xlq.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cah.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://whh.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cwf.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jyq.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pzx.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dfo.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://jff.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nea.nwbrower.top

[H10] 资源自动释放
来源：http://kct.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rga.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qdi.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bjj.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qas.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wym.ppjwa.cn

Go:   defer f.Close()
来源：http://ehz.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://goo.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lgm.shangyingyoupin.top

================================================================================
来源：http://fok.haohaochexian.top

I. 正则表达式
来源：http://sdo.pycfn.com

================================================================================
来源：http://tfe.pycfn.com

[I01] 判断是否匹配
来源：http://smr.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://srz.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wye.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://fqc.jianghu66.top

TS:   /\d+/.test(s)
来源：http://zxy.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kmx.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bqz.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://mkc.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ybp.yueranfly.top

[I02] 提取所有匹配
来源：http://xsb.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://vzi.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sfq.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gjp.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://xnq.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dcx.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ica.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://gqk.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qbs.xinyue.icu

[I03] 提取捕获分组
来源：http://pox.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rcn.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://usl.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lbj.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://czf.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nwz.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vgv.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iqj.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hsv.c1oappe.top

[I04] 正则替换
来源：http://tkk.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sla.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nzh.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://evb.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xrr.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ras.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tau.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fdj.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://egu.sjlbkw.cn

[I05] 按正则拆分
来源：http://nmk.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hsn.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wsg.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://tyk.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://azx.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://ukr.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vwy.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://scd.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bkl.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sae.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lov.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nje.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbv.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agj.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pgm.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xet.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tdc.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xxq.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://dsa.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://euq.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vnw.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uze.jiagoushi.top

TS:   /error/gim
来源：http://srh.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mab.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jiv.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://rtd.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ajz.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://azv.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pvw.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eth.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uaj.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xmq.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oeu.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zfq.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jax.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qns.yvedp.cn

================================================================================
来源：http://ino.yj20258888.top

J. 日期与时间
来源：http://tjp.hcnkem.com

================================================================================
来源：http://vbw.gzhubu.top

[J01] 获取当前时间
来源：http://ymc.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vtd.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uvk.uphjek.com

JS:   new Date();  Date.now()
来源：http://ktw.cheryme.top

TS:   new Date();  Date.now()
来源：http://sth.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bus.shzxlz.cn

Go:   time.Now()
来源：http://blj.zhengqikj.top

Ruby: Time.now
来源：http://ome.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvz.hcnkem.com

[J02] 格式化输出
来源：http://uoe.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bqb.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jbj.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nel.snrcjt.cn

TS:   d.toISOString()
来源：http://pnr.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://teg.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hvm.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mrc.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://itv.ppjwa.cn

[J03] 字符串解析为日期
来源：http://qno.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wqz.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://efl.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://vpm.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://tgg.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://glu.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zky.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://omy.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cez.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://cjt.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://huu.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lkj.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wia.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ttq.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sfq.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wsg.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fxu.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rxm.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://tzd.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://vjc.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://rch.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dlb.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ztb.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://vwq.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mgm.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://brl.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://exw.kuanghao11.cn

[J06] 计算两时间之差
来源：http://ejs.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://lsf.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://quq.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://soj.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jln.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xfp.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://jwn.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://asu.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://rgv.ivvv.top

[J07] 比较两个日期
来源：http://yfp.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://cen.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wxy.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fji.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://nbo.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iam.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://peg.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://tto.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://obq.aibaodan.cn

[J08] 提取年月日与星期
来源：http://oil.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rno.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ekl.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hfr.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xis.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rww.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sfo.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://idh.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mah.sxryk.cn

[J09] 时区处理
来源：http://yii.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://epp.ywan-chungtsiang.top


<!-- 参考信息 -->