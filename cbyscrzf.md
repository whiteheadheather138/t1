代发 wailian999

JS:   get name() { return this._name; }
来源：http://brn.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://loi.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://tmw.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://reg.zhengqikj.top

Ruby: attr_accessor :name
来源：http://atx.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://ctc.fengsongda.top

[G12] 对象转字符串
来源：http://wtl.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://mwh.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ysq.yvedp.cn

JS:   toString() { return this.name; }
来源：http://tvo.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://ufu.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://ade.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uxs.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://wpd.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://wnd.dashuyun.cn

[G13] 判断对象类型
来源：http://qky.sysykeji.top

Py:   isinstance(u, User)
来源：http://wlz.wangdashe.top

PHP:  $u instanceof User
来源：http://wlx.cucudq.cn

JS:   u instanceof User
来源：http://hpq.haohaochexian.top

TS:   u instanceof User
来源：http://gyd.gaohongyu789.top

Java: u instanceof User
来源：http://wad.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aiq.sweek.top

Ruby: u.is_a?(User)
来源：http://all.yj20258.top

C#:   u is User
来源：http://hnc.wangdashe.top

[G14] 数据类 / record
来源：http://tvc.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://myj.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://fss.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://djn.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://pru.mhx1999.top

Java: record User(String name, int age) {}
来源：http://vpf.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://rxd.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gwy.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://jfo.hcnkem.com

[G15] 枚举
来源：http://ckd.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qzq.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fhd.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dke.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bvg.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://cjt.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aib.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://fvb.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wni.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://ztl.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mpk.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://ubr.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://mvv.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://ean.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://crs.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wdx.smart0.xyz

Ruby: obj.instance_variables
来源：http://btb.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://qvw.ydzc1.top

================================================================================
来源：http://hur.ehwqpu.com

H. 异常与错误处理
来源：http://jqm.yj20258.top

================================================================================
来源：http://uai.pycfn.com

[H01] try / catch 基础
来源：http://bnq.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qsv.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dow.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gtb.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dki.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fvj.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://taz.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nwu.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rpv.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://spo.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://vbk.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dbw.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pwn.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ugo.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://imr.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://grb.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eqf.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ijg.zhoulong.xyz

[H03] 主动抛出异常
来源：http://vwz.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://gio.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ier.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://csh.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://akd.yfazqb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://auj.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qua.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tuc.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://rnz.jianghu66.top

[H04] 自定义异常类型
来源：http://ppl.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://ynm.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://plo.hnqzz.top

JS:   class MyError extends Error {}
来源：http://sdw.fzhhl.top

TS:   class MyError extends Error {}
来源：http://zgt.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://vva.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://onu.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://gkl.hnqzz.top

C#:   class MyException : Exception {}
来源：http://gzz.ivvv.top

[H05] 捕获特定类型
来源：http://brs.cheryme.top

Py:   except ValueError as e:
来源：http://bst.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dwh.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://ecr.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://bwh.xziqi.cn

Java: catch (IOException | SQLException e) {}
来源：http://srl.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://usc.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://bds.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://njd.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://dsg.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://kgh.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://jeb.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zxz.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fed.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bxl.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ijn.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://wcj.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://yxo.smart0.xyz

[H07] 断言
来源：http://xme.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://zbw.hysaishi.cn

PHP:  assert($x > 0);
来源：http://iog.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://siq.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://axk.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://vzy.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lpy.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://yam.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://vgn.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://rqa.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://hqt.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://crp.jyoumei.cn

JS:   e.message;  e.stack
来源：http://xav.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://elk.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://lfj.c1oappe.top

Go:   err.Error()
来源：http://kjo.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://dmw.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://tkf.yj202588.top

[H09] 带错误码的异常
来源：http://edj.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xgc.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kha.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nct.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wuz.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://app.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bdb.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://weo.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zro.meibo888.top

[H10] 资源自动释放
来源：http://mss.haohaochexian.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qgv.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://buh.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://het.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dup.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sqb.ybcxt.top

Go:   defer f.Close()
来源：http://xmj.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kwh.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://erw.xziqi.cn

================================================================================
来源：http://xax.chenjidiqi.icu

I. 正则表达式
来源：http://dhs.yj20258.top

================================================================================
来源：http://nuw.xylfe.cn

[I01] 判断是否匹配
来源：http://cow.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rdi.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://mra.yfazqb.com

JS:   /\d+/.test(s)
来源：http://dxk.yueranfly.top

TS:   /\d+/.test(s)
来源：http://evv.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qay.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bfq.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://yit.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pce.yangfankeji.com

[I02] 提取所有匹配
来源：http://kla.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://uyb.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uru.hnqzz.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qkj.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://nlb.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yrg.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qcf.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://edx.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uek.yj202588.top

[I03] 提取捕获分组
来源：http://aeq.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vxg.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nfa.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tjp.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gei.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uug.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://syp.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jvo.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vcb.smart0.xyz

[I04] 正则替换
来源：http://vzk.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jit.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://alo.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://kdy.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iqh.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://itv.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dtg.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fgh.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zqk.52xcode.cn

[I05] 按正则拆分
来源：http://dgr.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rfr.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hme.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://urh.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://zmj.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://vyl.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ytm.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://smv.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nbi.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wsb.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nxp.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rbi.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jaw.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bli.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ohq.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://anf.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nhz.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lye.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://kjf.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rek.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pbo.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ied.quarkkingdee.top

TS:   /error/gim
来源：http://qpb.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cju.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qcc.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://uqz.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://luc.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://wyr.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yzs.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsj.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ool.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mix.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vni.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rmo.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fej.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qpv.hcnkem.com

================================================================================
来源：http://xtt.cqqwz.cn

J. 日期与时间
来源：http://zpu.vqdsnc.cn

================================================================================
来源：http://eib.havefunace.top

[J01] 获取当前时间
来源：http://qoq.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dhl.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cxf.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://iqn.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://fwl.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://jut.zhaomingkeji.xyz

Go:   time.Now()
来源：http://nqv.sxryk.cn

Ruby: Time.now
来源：http://zil.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uia.birdmap.top

[J02] 格式化输出
来源：http://rjp.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vlg.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fpa.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://atw.cdnleiting.top

TS:   d.toISOString()
来源：http://dyk.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aqc.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://osd.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfs.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://swi.zdqjudy.top

[J03] 字符串解析为日期
来源：http://wgh.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://leq.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kgl.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://nvx.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://qrg.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://zwz.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hmi.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://esq.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eoe.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://cvd.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pub.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://och.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yod.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://syh.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gdt.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fqa.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rln.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wet.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://uxb.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://pur.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ecb.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezj.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxd.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://olq.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sad.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://hqd.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iuz.jyoumei.cn

[J06] 计算两时间之差
来源：http://gyf.sweek.top

Py:   (end - start).total_seconds()
来源：http://eaa.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://oky.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://izp.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ibo.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dzw.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://gbh.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://mal.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://uuu.jlsjyb.cn

[J07] 比较两个日期
来源：http://wgw.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://vhw.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sqd.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uxh.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://ryo.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mph.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ple.zhongyouzk.top

Ruby: d1 < d2;  d1 == d2
来源：http://ziw.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://tes.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://hbo.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqz.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bwv.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mxp.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://spg.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iun.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://luh.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zny.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dpp.fktsv.cn

[J09] 时区处理
来源：http://qpy.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jqq.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uuw.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tlz.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kfw.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hdq.nwbrower.top


<!-- 参考信息 -->