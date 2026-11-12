代发 wailian999

JS:   get name() { return this._name; }
来源：http://qpa.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://wku.yuxming.cn

Java: public String getName() { return name; }
来源：http://hgt.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ebj.uphjek.com

Ruby: attr_accessor :name
来源：http://tqz.sxryk.cn

C#:   public string Name { get; set; }
来源：http://mqh.xinyue.icu

[G12] 对象转字符串
来源：http://rru.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://hnm.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dbo.fzhhl.top

JS:   toString() { return this.name; }
来源：http://pcv.cucudq.cn

TS:   toString(): string { return this.name; }
来源：http://pby.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://bfr.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://swv.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://sfi.pycfn.com

C#:   public override string ToString() => Name;
来源：http://kcg.tian-w.cn

[G13] 判断对象类型
来源：http://ilc.fktsv.cn

Py:   isinstance(u, User)
来源：http://qgm.pycfn.com

PHP:  $u instanceof User
来源：http://ibs.tianlin.xyz

JS:   u instanceof User
来源：http://nsk.hywenlv.cn

TS:   u instanceof User
来源：http://kqs.tarul.cn

Java: u instanceof User
来源：http://lex.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://znr.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://rnm.xingfuxueyuan.xyz

C#:   u is User
来源：http://eqj.chenlongwang.top

[G14] 数据类 / record
来源：http://kcb.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tlk.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://nvr.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qoz.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://obx.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://tka.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://ela.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qfc.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://wdt.52xcode.cn

[G15] 枚举
来源：http://rcz.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://unj.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://xdz.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fdd.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://akp.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://jfy.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://clf.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://fgh.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qtg.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://dgt.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qco.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://rcu.daria6918.cn

JS:   Object.entries(obj)
来源：http://lsh.hywenlv.cn

TS:   Object.entries(obj)
来源：http://und.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lpj.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://eik.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://xuc.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://ovt.gaohongyu789.top

================================================================================
来源：http://jfx.52xcode.cn

H. 异常与错误处理
来源：http://xss.nanxuanxn.top

================================================================================
来源：http://xvb.ydzc1.top

[H01] try / catch 基础
来源：http://uav.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rtj.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tco.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ete.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uov.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xvp.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pah.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wmt.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uzm.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://hmy.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://ica.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://hdo.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rbf.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://apw.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://qrm.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://imw.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://and.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iuh.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://rlw.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://moc.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zgi.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://gdo.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://apu.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://her.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lfe.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xkc.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://jxz.aibaodan.cn

[H04] 自定义异常类型
来源：http://gmh.yongpay.top

Py:   class MyError(Exception): pass
来源：http://imc.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://vli.ydzc1.top

JS:   class MyError extends Error {}
来源：http://cml.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://gcq.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://dmt.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qny.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://fuy.vehdjk.com

C#:   class MyException : Exception {}
来源：http://viz.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://spr.gzhubu.top

Py:   except ValueError as e:
来源：http://oxa.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dnj.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://kwn.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://zqk.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://cgt.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mmm.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://cve.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qwd.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://rvo.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://gam.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://hxi.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://gkp.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zlv.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qrm.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fky.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://cah.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://wiv.daxiang520.top

[H07] 断言
来源：http://srz.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://rqm.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://gsr.tian-w.cn

JS:   console.assert(x > 0);
来源：http://ahf.zycfv.cn

TS:   console.assert(x > 0);
来源：http://zzv.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://jkq.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zyg.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://zxd.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://olo.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://qhe.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://skw.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xat.yueranfly.top

JS:   e.message;  e.stack
来源：http://pum.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tnj.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lne.sjlbkw.cn

Go:   err.Error()
来源：http://lhl.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://pnl.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://jgh.aibaodan.cn

[H09] 带错误码的异常
来源：http://vgq.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fvm.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ctd.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eyt.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tuk.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cus.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tux.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://way.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gss.ctjpmb.com

[H10] 资源自动释放
来源：http://gsf.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gmw.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uob.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jex.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jbt.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fdh.c1oappe.top

Go:   defer f.Close()
来源：http://tks.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xnb.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xuu.jqgufenzy.top

================================================================================
来源：http://qtl.tanke756.top

I. 正则表达式
来源：http://eoj.cheryme.top

================================================================================
来源：http://kxu.fengsongda.top

[I01] 判断是否匹配
来源：http://khj.hywenlv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ryp.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://zfr.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://fow.fehbvm.com

TS:   /\d+/.test(s)
来源：http://dkl.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xbm.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tfk.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://vib.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zau.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://uip.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://gev.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pyy.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://icw.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://cei.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qql.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://erm.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://bgs.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pxf.svipenyu.cn

[I03] 提取捕获分组
来源：http://lvr.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zuk.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hqh.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cff.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zlr.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gje.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vcy.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jjs.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ucj.316326.xyz

[I04] 正则替换
来源：http://bch.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://qhz.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xll.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://uds.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nch.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nvp.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://azi.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xwy.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xvk.snrcjt.cn

[I05] 按正则拆分
来源：http://hyh.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://shg.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ejt.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://jyc.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://qwx.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://etu.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jgo.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://yco.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tvh.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://los.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hau.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ebn.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mbm.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmk.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lht.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ckq.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zbu.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iph.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://clq.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cpx.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lob.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ncl.aibaodan.cn

TS:   /error/gim
来源：http://uju.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ulg.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zvp.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://mwf.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iqc.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://rvn.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://frj.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uar.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nwh.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jfb.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xad.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zir.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cuo.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jva.gogol.net.cn

================================================================================
来源：http://vhc.yvedp.cn

J. 日期与时间
来源：http://jne.vehdjk.com

================================================================================
来源：http://whw.wangshuangyany.cn

[J01] 获取当前时间
来源：http://gyy.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aoz.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://new.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://xeg.ivvv.top

TS:   new Date();  Date.now()
来源：http://lab.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bzn.xylfe.cn

Go:   time.Now()
来源：http://naa.gogol.net.cn

Ruby: Time.now
来源：http://mvc.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zpj.c1oappe.top

[J02] 格式化输出
来源：http://jdh.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ycw.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://prx.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ziz.hesvh.cn

TS:   d.toISOString()
来源：http://olh.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lda.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gmf.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gum.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lux.uphjek.com

[J03] 字符串解析为日期
来源：http://zse.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oso.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://svr.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://gzl.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://mbb.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://ipv.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mxl.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://bdu.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yis.sxryk.cn

[J04] 时间戳与日期互转
来源：http://qny.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uup.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qeb.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hrb.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qfx.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bnd.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tvt.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mpd.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bim.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://jrq.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://rjq.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://mnx.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mnw.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sxt.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://qqx.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sjy.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://lwg.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://xxl.zhijiandao.cn

[J06] 计算两时间之差
来源：http://bat.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://xwz.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://xsg.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sxk.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://akx.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ueg.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://llu.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://xap.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://fqn.xuetiantiany.cn

[J07] 比较两个日期
来源：http://btr.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://qcj.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uzb.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xru.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ser.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wzi.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rbm.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://awl.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://wvp.bjfxy.top

[J08] 提取年月日与星期
来源：http://qbd.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eiq.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qrh.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dfp.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kjk.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tcw.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wyh.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wnj.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kiq.epnwcf.com

[J09] 时区处理
来源：http://ozq.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zuv.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://czb.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nkl.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckb.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lcq.ydzc1.top


<!-- 参考信息 -->