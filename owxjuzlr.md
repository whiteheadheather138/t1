代发 wailian999

C#:   public / protected / private / internal
来源：http://npi.yangfankeji.com

[G11] getter / setter
来源：http://ozr.tarul.cn

Py:   @property 与 @x.setter
来源：http://nxd.jqgufenzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jur.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://zkd.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://sxh.hywenlv.cn

Java: public String getName() { return name; }
来源：http://lme.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vyr.ehwqpu.com

Ruby: attr_accessor :name
来源：http://qqp.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://oyl.52xcode.cn

[G12] 对象转字符串
来源：http://ddi.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://nzj.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lnx.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://cqh.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://hzb.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://qnk.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ebi.jianghu66.top

Ruby: def to_s; @name; end
来源：http://bro.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://chr.0kj1m.cn

[G13] 判断对象类型
来源：http://atk.ydzc1.top

Py:   isinstance(u, User)
来源：http://bwj.yj20258888.top

PHP:  $u instanceof User
来源：http://byq.svipenyu.cn

JS:   u instanceof User
来源：http://jcp.gzhubu.top

TS:   u instanceof User
来源：http://clb.epnwcf.com

Java: u instanceof User
来源：http://kje.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ssd.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://xyt.hnqzz.top

C#:   u is User
来源：http://ndu.chenlongwang.top

[G14] 数据类 / record
来源：http://xaq.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tvt.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://hac.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vvu.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://ppe.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://ztj.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://dug.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ptr.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://bgv.xziqi.cn

[G15] 枚举
来源：http://fwo.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://adt.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ymo.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cjj.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cqk.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://tyq.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uit.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://qae.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mvj.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://nzq.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xsl.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://wnl.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://rgy.zycfv.cn

TS:   Object.entries(obj)
来源：http://erh.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pxy.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://iyb.yonumen.top

Ruby: obj.instance_variables
来源：http://kfj.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://hzh.yueranfly.top

================================================================================
来源：http://ysp.birdmap.top

H. 异常与错误处理
来源：http://mik.gzhubu.top

================================================================================
来源：http://htn.bbcook.cn

[H01] try / catch 基础
来源：http://rch.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uqa.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gtq.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://glx.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bil.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://glh.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tdj.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vwm.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hty.tanke756.top

[H02] finally / ensure 收尾
来源：http://iqd.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://efo.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rxu.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uxx.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pak.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ppj.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fqp.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qki.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://leo.vqdsnc.cn

[H03] 主动抛出异常
来源：http://dmn.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://uke.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tzz.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://xtr.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://zjb.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://raw.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qsw.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wfd.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://xpt.hysaishi.cn

[H04] 自定义异常类型
来源：http://tid.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://bjf.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://bcf.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://inw.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://hok.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://wyr.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mui.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://atj.bbcook.cn

C#:   class MyException : Exception {}
来源：http://ajk.hnxiangtu.top

[H05] 捕获特定类型
来源：http://gza.0kj1m.cn

Py:   except ValueError as e:
来源：http://elu.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lvp.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://rbr.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://mmx.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://mzx.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rne.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://sbm.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mtj.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://aqm.xuanzx.com

Py:   value = d.get("k") or default
来源：http://zpr.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://gsq.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://dvv.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://bqi.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://faf.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cyq.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://nil.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://ibd.hammf.cn

[H07] 断言
来源：http://iuw.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://izc.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://hwl.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://pxn.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://zqk.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://lrb.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tlo.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://hyd.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://nfo.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://lar.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://gci.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jfd.ctjpmb.com

JS:   e.message;  e.stack
来源：http://lio.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rhr.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eqx.nwbrower.top

Go:   err.Error()
来源：http://qku.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://mib.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://xqx.tanke756.top

[H09] 带错误码的异常
来源：http://mor.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nlm.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bwj.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tnx.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pto.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hts.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ema.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://qgh.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://dlm.c1oappe.top

[H10] 资源自动释放
来源：http://evc.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vuv.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://liz.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jcd.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gdk.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://idb.xylfe.cn

Go:   defer f.Close()
来源：http://yjv.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xnw.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdj.shanyushiyangkeji.top

================================================================================
来源：http://uvy.jinghuilouyu.cn

I. 正则表达式
来源：http://zif.tianlin.xyz

================================================================================
来源：http://agh.hysaishi.cn

[I01] 判断是否匹配
来源：http://zrk.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fak.tianlin.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://twp.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://jcu.hesvh.cn

TS:   /\d+/.test(s)
来源：http://xig.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbn.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://flz.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://rfl.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ncj.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://asr.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://kdt.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nnk.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://myw.316326.xyz

TS:   s.match(/\d+/g)
来源：http://ftv.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rux.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yhv.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://dmw.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://trv.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://dgj.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ylt.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jlv.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lpt.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uds.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fae.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hqd.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hmw.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://quo.jiagoushi.top

[I04] 正则替换
来源：http://nqe.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ulp.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nhy.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://okm.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sxg.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://ykj.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uvg.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yjp.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oew.hysaishi.cn

[I05] 按正则拆分
来源：http://xmu.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ace.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://agg.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://cba.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://sno.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://bqx.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cgm.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://sgt.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ujg.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://trj.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://stn.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://buz.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nqz.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://epw.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xuy.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://opp.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qoa.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jis.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://uok.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yur.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://etm.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iud.guowangkeji.top

TS:   /error/gim
来源：http://zhs.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://unt.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bal.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://zoj.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://alp.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://ahb.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bnt.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mgm.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rpb.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kte.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fqa.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wcr.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tto.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yvf.hesvh.cn

================================================================================
来源：http://bau.yuanzhike.top

J. 日期与时间
来源：http://mgp.shanyushiyangtech.top

================================================================================
来源：http://buw.guowangkeji.top

[J01] 获取当前时间
来源：http://eot.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xrt.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://obl.redwolf501.top

JS:   new Date();  Date.now()
来源：http://jrr.yj202588.top

TS:   new Date();  Date.now()
来源：http://tac.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wnk.xuanzx.com

Go:   time.Now()
来源：http://adi.nanxinkj.top

Ruby: Time.now
来源：http://pct.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vgh.9152youxi.cn

[J02] 格式化输出
来源：http://xwo.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lhu.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pov.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://way.52xcode.cn

TS:   d.toISOString()
来源：http://jmx.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sye.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vzj.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fiu.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gfk.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://awk.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dgu.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jik.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://tyu.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://nnj.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://iuc.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jxc.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://fsq.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iim.yj20258888.top

[J04] 时间戳与日期互转
来源：http://nts.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lcv.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fio.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vkm.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://rtf.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rxc.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fis.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hvu.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vio.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://bhy.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://vgm.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://dmi.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sjy.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rjx.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://bxm.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bol.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://vwj.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://wff.havefunace.top

[J06] 计算两时间之差
来源：http://wdj.meibo888.top

Py:   (end - start).total_seconds()
来源：http://cdu.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://pap.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kgj.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://exo.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://aqg.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://juk.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://zvq.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://zmb.aibaodan.cn

[J07] 比较两个日期
来源：http://hot.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://gti.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lnn.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://wbl.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://hxe.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ctq.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ynr.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://dqc.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://xzd.smart0.xyz

[J08] 提取年月日与星期
来源：http://ltd.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wci.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zhs.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kwm.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qra.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kne.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mxl.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ybt.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ciq.sweek.top

[J09] 时区处理
来源：http://hsm.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hmv.zhixingplan.top


<!-- 参考信息 -->