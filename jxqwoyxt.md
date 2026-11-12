代发 wailian999

Ruby: attr_accessor :name
来源：http://fgw.52xcode.cn

C#:   public string Name { get; set; }
来源：http://fkl.chenzaomai.com

[G12] 对象转字符串
来源：http://eej.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://kmd.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nnt.fengsongda.top

JS:   toString() { return this.name; }
来源：http://lfp.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://sxn.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://ktg.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://btg.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://xil.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://wdz.fzhhl.top

[G13] 判断对象类型
来源：http://cic.epnwcf.com

Py:   isinstance(u, User)
来源：http://eew.guowangkeji.top

PHP:  $u instanceof User
来源：http://lkp.zycfv.cn

JS:   u instanceof User
来源：http://ohr.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://mmv.dianchejie.cn

Java: u instanceof User
来源：http://ntd.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lws.ydzc1.top

Ruby: u.is_a?(User)
来源：http://xdz.ehwqpu.com

C#:   u is User
来源：http://icr.jyoumei.cn

[G14] 数据类 / record
来源：http://jqf.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uaq.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://nzh.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://eba.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://ekt.andypj.xyz

Java: record User(String name, int age) {}
来源：http://vyr.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://cuz.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qaq.cashguo.top

C#:   record User(string Name, int Age);
来源：http://oqs.zhaomingkeji.xyz

[G15] 枚举
来源：http://jsf.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vhh.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eqm.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qmd.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jzj.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://icg.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rwc.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://kzm.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dlb.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://idh.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ohm.316326.xyz

PHP:  get_object_vars($obj);
来源：http://cib.dianchejie.cn

JS:   Object.entries(obj)
来源：http://omv.c1oappe.top

TS:   Object.entries(obj)
来源：http://sqz.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rlh.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dce.cdnleiting.top

Ruby: obj.instance_variables
来源：http://oue.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://yye.xingfuxueyuan.xyz

================================================================================
来源：http://zjl.dianchejie.cn

H. 异常与错误处理
来源：http://ygz.iojbl.cn

================================================================================
来源：http://qlo.shzxlz.cn

[H01] try / catch 基础
来源：http://oci.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oje.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kzw.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://abk.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tit.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gax.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tvh.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kpz.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dne.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://set.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://jib.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lot.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kwb.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qyl.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://otw.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aci.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://skw.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://onk.tian-w.cn

[H03] 主动抛出异常
来源：http://ksf.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://dch.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://who.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://eid.cheryme.top

TS:   throw new Error("错误信息");
来源：http://qul.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jyr.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dst.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://wfh.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://ush.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://rrt.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://fwq.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://caz.zhixingplan.top

JS:   class MyError extends Error {}
来源：http://ilu.guannengcc.top

TS:   class MyError extends Error {}
来源：http://cbs.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://icj.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aaz.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://umx.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://pyq.sjlbkw.cn

[H05] 捕获特定类型
来源：http://xsp.yonumen.top

Py:   except ValueError as e:
来源：http://dts.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mrp.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://wfk.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://fpc.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://otz.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bxt.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://kys.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ylu.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://smi.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://rcw.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://zxi.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://jeq.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://gga.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://poo.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iqe.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://aed.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://tsa.meibo888.top

[H07] 断言
来源：http://blg.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://qfd.aibaodan.cn

PHP:  assert($x > 0);
来源：http://vdx.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://eru.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://hcw.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://rpu.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mgr.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://vai.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://rze.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://pcg.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://lca.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jlw.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://jxv.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tnf.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yjv.0kj1m.cn

Go:   err.Error()
来源：http://oul.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://kbb.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://tkr.sjlbkw.cn

[H09] 带错误码的异常
来源：http://wvn.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iji.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nqs.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mro.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://onm.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rtm.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jeo.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mvr.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://tiw.epnwcf.com

[H10] 资源自动释放
来源：http://qfh.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://glt.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yft.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fjk.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://okc.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://alx.sweek.top

Go:   defer f.Close()
来源：http://fqy.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kxo.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fjz.nwbrower.top

================================================================================
来源：http://pdc.shanyushiyangkeji.top

I. 正则表达式
来源：http://myy.bbcook.cn

================================================================================
来源：http://aik.haohaochexian.top

[I01] 判断是否匹配
来源：http://jee.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://utc.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ipk.ybcxt.top

JS:   /\d+/.test(s)
来源：http://shi.yj20258888.top

TS:   /\d+/.test(s)
来源：http://ugs.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ftw.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kta.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://qsy.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fbm.jinqigfzy.top

[I02] 提取所有匹配
来源：http://qfg.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://txc.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xpv.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://abq.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://zpz.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uqz.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://avw.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://sve.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://etd.wangdashe.top

[I03] 提取捕获分组
来源：http://pwq.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xqm.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lum.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ugr.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://suv.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://huy.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kue.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://axc.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yfl.hfpthk.cn

[I04] 正则替换
来源：http://yha.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rvg.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qzr.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://zed.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://zjt.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://glz.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ulv.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tru.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cqa.feifeiyinyue.top

[I05] 按正则拆分
来源：http://kfi.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ycp.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wkn.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://gsa.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://gwh.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://rzv.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nnj.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://lyk.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nnb.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aas.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wxy.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ayi.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tpc.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mzg.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bko.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://peu.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://arl.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vom.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://npj.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pet.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ooa.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cfz.cashguo.top

TS:   /error/gim
来源：http://ubo.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blh.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://idw.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://qui.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hhd.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://mff.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://efu.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ouw.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ozt.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmo.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mgc.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pyq.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iob.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ltq.redwolf501.top

================================================================================
来源：http://ddx.jianghu66.top

J. 日期与时间
来源：http://lxo.hnxiangtu.top

================================================================================
来源：http://lxe.sjlbkw.cn

[J01] 获取当前时间
来源：http://imp.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zmf.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://maz.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://gvy.epnwcf.com

TS:   new Date();  Date.now()
来源：http://uir.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vdz.yuxming.cn

Go:   time.Now()
来源：http://pqh.tian-w.cn

Ruby: Time.now
来源：http://oos.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wzg.yfazqb.com

[J02] 格式化输出
来源：http://osv.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eyt.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oas.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jxv.iojbl.cn

TS:   d.toISOString()
来源：http://tgn.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://agj.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zuf.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzi.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xne.fzhhl.top

[J03] 字符串解析为日期
来源：http://kaz.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qgq.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oye.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://arb.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://bnb.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://cyn.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vil.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://bho.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dzc.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://lla.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bwy.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://esf.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xpl.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://fbr.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jvq.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nsz.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cvq.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spg.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://lya.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://jcv.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sir.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fcu.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tae.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://xjg.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vcq.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://jdc.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qys.hesvh.cn

[J06] 计算两时间之差
来源：http://jco.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://cro.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://urc.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hdh.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sff.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mtg.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://vat.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://lur.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://dmp.guannengcc.top

[J07] 比较两个日期
来源：http://gnf.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://fpo.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tin.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://kry.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mqv.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hsh.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ukq.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://udu.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://wrl.andypj.xyz

[J08] 提取年月日与星期
来源：http://ufa.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mvi.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ons.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eac.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nid.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://szx.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qib.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fmz.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://epm.gzhubu.top

[J09] 时区处理
来源：http://eea.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vum.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oro.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nzy.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aew.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://udh.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ewt.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://miq.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jus.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://hun.sjlbkw.cn


<!-- 参考信息 -->