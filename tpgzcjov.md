代发 wailian999

TS:   public / protected / private
来源：http://rkt.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://xxf.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bva.52xcode.cn

Ruby: public / protected / private
来源：http://pgy.zdbjq.cn

C#:   public / protected / private / internal
来源：http://drb.yvedp.cn

[G11] getter / setter
来源：http://xih.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://ssl.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fym.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://vpe.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://mvk.vehdjk.com

Java: public String getName() { return name; }
来源：http://suu.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://cwz.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://mjw.yvedp.cn

C#:   public string Name { get; set; }
来源：http://pqt.xylfe.cn

[G12] 对象转字符串
来源：http://ijt.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://uem.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gxd.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://quu.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://qrf.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://dnp.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://ezx.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://aml.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://omd.svipenyu.cn

[G13] 判断对象类型
来源：http://bff.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://oda.yuxming.cn

PHP:  $u instanceof User
来源：http://osb.zhixingplan.top

JS:   u instanceof User
来源：http://mhx.yanxiufei.cn

TS:   u instanceof User
来源：http://xxj.shzxlz.cn

Java: u instanceof User
来源：http://poq.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rlh.yfazqb.com

Ruby: u.is_a?(User)
来源：http://vwp.fengsongda.top

C#:   u is User
来源：http://pcp.sweek.top

[G14] 数据类 / record
来源：http://lrn.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qjr.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://rog.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://izl.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://any.fzhhl.top

Java: record User(String name, int age) {}
来源：http://ztf.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://bgv.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://flr.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://yow.ybcxt.top

[G15] 枚举
来源：http://xvn.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ehm.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gar.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ggb.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://czd.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://cqx.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aub.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://ioe.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tkv.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://med.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qea.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://gtw.yonumen.top

JS:   Object.entries(obj)
来源：http://rcf.hammf.cn

TS:   Object.entries(obj)
来源：http://yln.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tfw.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fgx.shzxlz.cn

Ruby: obj.instance_variables
来源：http://pcg.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://xbv.yanxiufei.cn

================================================================================
来源：http://znk.snrcjt.cn

H. 异常与错误处理
来源：http://cnv.bbcook.cn

================================================================================
来源：http://hfh.sweek.top

[H01] try / catch 基础
来源：http://goi.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bdm.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ptg.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fab.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qcj.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pzb.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nki.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pvy.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jqf.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://ado.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fzg.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://vsq.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jgy.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://wvu.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://edd.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ahh.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qpx.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cbx.cdnleiting.top

[H03] 主动抛出异常
来源：http://tjx.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://fer.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vll.tarul.cn

JS:   throw new Error("错误信息");
来源：http://exe.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://nhs.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://roo.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://krw.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://uhd.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://ets.haohaochexian.top

[H04] 自定义异常类型
来源：http://rfi.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://gry.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://mfb.yj202588.top

JS:   class MyError extends Error {}
来源：http://fzi.cheryme.top

TS:   class MyError extends Error {}
来源：http://mah.kuanghao11.cn

Java: class MyException extends RuntimeException {}
来源：http://ylp.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sia.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://muv.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://vzy.xinyue.icu

[H05] 捕获特定类型
来源：http://hfa.zhijiandao.cn

Py:   except ValueError as e:
来源：http://wmx.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gpg.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://nao.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://kdt.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://vul.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gbf.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://hfm.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rfx.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://tcf.andypj.xyz

Py:   value = d.get("k") or default
来源：http://mcp.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://hnv.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gqd.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fyr.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://clx.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yrc.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://tbk.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://eir.sweek.top

[H07] 断言
来源：http://exw.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://xpx.yj20258888.top

PHP:  assert($x > 0);
来源：http://luk.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://mxb.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://ocy.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://fcv.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xzr.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://urf.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://fvv.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://hlc.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://nvu.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bqs.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://krb.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://itr.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yat.zhengqikj.top

Go:   err.Error()
来源：http://bnc.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://fmx.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://kpu.fehbvm.com

[H09] 带错误码的异常
来源：http://wma.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ims.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hfp.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lww.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sua.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lqp.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pnc.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://yor.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://njp.yueranfly.top

[H10] 资源自动释放
来源：http://epr.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ahk.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://feq.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bkb.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qnn.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nmb.dianchejie.cn

Go:   defer f.Close()
来源：http://ybd.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ndn.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bhe.svipenyu.cn

================================================================================
来源：http://agw.chenjidiqi.icu

I. 正则表达式
来源：http://oos.tian-w.cn

================================================================================
来源：http://cfc.yfazqb.com

[I01] 判断是否匹配
来源：http://lnu.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://beb.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://ylv.yueranfly.top

JS:   /\d+/.test(s)
来源：http://gws.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://vvc.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://abh.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nlu.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://prd.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gbu.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://hnw.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://qrh.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lsp.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://biy.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://pip.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jpx.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uqe.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://eso.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jqf.sjlbkw.cn

[I03] 提取捕获分组
来源：http://wgn.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://efe.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wze.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lqw.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qxm.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ors.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pax.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://klo.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ugz.shuidangran.top

[I04] 正则替换
来源：http://xej.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://unp.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cmc.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mgw.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://ziz.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qeq.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hrj.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xuq.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ijj.yangfankeji.com

[I05] 按正则拆分
来源：http://lpy.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://xcg.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rko.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://pnf.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://rpf.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://ihj.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mqr.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ozt.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://thn.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xtp.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ppd.cdnleiting.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tlj.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ody.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvt.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nrs.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://exx.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vka.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gzn.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://wxv.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eji.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wec.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eou.fzhhl.top

TS:   /error/gim
来源：http://wcq.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qtz.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bih.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://uhx.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iut.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://jsm.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fgj.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ywd.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gfe.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtx.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fvj.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vvl.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yul.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzo.quarkkingdee.top

================================================================================
来源：http://vee.ehwqpu.com

J. 日期与时间
来源：http://itb.dashuyun.cn

================================================================================
来源：http://ixe.jqgfzy.top

[J01] 获取当前时间
来源：http://gfu.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qsc.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://plz.bjfxy.top

JS:   new Date();  Date.now()
来源：http://hmj.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://nkl.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nwm.tian-w.cn

Go:   time.Now()
来源：http://xhx.aibaodan.cn

Ruby: Time.now
来源：http://bhf.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wml.zhiwuduotai.top

[J02] 格式化输出
来源：http://ove.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rxr.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://anm.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rxa.tanke756.top

TS:   d.toISOString()
来源：http://vsk.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://swb.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nzu.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vvx.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bjg.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://jtt.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ilv.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kvf.havefunace.top

JS:   new Date("2024-01-02")
来源：http://ciq.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://lzw.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lli.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vaj.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://pti.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nsd.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://uhv.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjg.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mqq.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zxb.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ojt.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mui.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iwa.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://epj.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hxu.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://vjl.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://gwb.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zcf.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oau.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gad.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://vtd.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mpc.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://ykv.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://dww.sweek.top

[J06] 计算两时间之差
来源：http://udg.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://uop.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://xcy.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xwg.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ypl.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hae.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://ftc.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://puq.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://qny.yj20258.top

[J07] 比较两个日期
来源：http://dww.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://vlq.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ayg.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://onc.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://jwh.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fuo.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rbe.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vnr.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://fsg.sweek.top

[J08] 提取年月日与星期
来源：http://eke.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://say.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wrf.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yvm.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pfw.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nba.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzu.hysaishi.cn


<!-- 参考信息 -->