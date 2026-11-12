代发 wailian999

JS:   get name() { return this._name; }
来源：http://cdl.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://qvp.0kj1m.cn

Java: public String getName() { return name; }
来源：http://sag.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uxj.xziqi.cn

Ruby: attr_accessor :name
来源：http://wle.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://jhn.uphjek.com

[G12] 对象转字符串
来源：http://rlu.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://mih.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wsp.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://llb.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://zgt.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://bxb.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://obk.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://oic.birdmap.top

C#:   public override string ToString() => Name;
来源：http://gcb.guannengcc.top

[G13] 判断对象类型
来源：http://ayl.ydzc1.top

Py:   isinstance(u, User)
来源：http://srb.sufxvd.cn

PHP:  $u instanceof User
来源：http://hrh.yj20258.top

JS:   u instanceof User
来源：http://nfk.sysykeji.top

TS:   u instanceof User
来源：http://lmx.cqqwz.cn

Java: u instanceof User
来源：http://rak.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wmy.hammf.cn

Ruby: u.is_a?(User)
来源：http://ejp.hammf.cn

C#:   u is User
来源：http://vjj.sxryk.cn

[G14] 数据类 / record
来源：http://jxo.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ebn.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://ffx.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nlq.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://ecs.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://mzy.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://kck.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://apq.birdmap.top

C#:   record User(string Name, int Age);
来源：http://wdl.tianlin.xyz

[G15] 枚举
来源：http://eqe.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hst.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dzw.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uvf.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dsx.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://svz.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tpm.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://noc.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pax.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://wdj.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kcx.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://wri.wangdashe.top

JS:   Object.entries(obj)
来源：http://dnt.wangdashe.top

TS:   Object.entries(obj)
来源：http://tqx.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aij.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ais.chenzaomai.com

Ruby: obj.instance_variables
来源：http://fas.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://jwb.yfazqb.com

================================================================================
来源：http://nwp.gaohongyu789.top

H. 异常与错误处理
来源：http://mqo.yvedp.cn

================================================================================
来源：http://siz.yongpay.top

[H01] try / catch 基础
来源：http://nol.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://riv.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kfc.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://psl.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xpk.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rmo.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tqy.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sls.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nrm.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://lzu.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qnl.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vqs.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uyz.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kdj.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://ocs.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bzp.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zsk.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rtr.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://mks.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://jkz.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tkm.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://ald.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://lsv.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://dte.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zzj.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://obn.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://mxh.chenlongwang.top

[H04] 自定义异常类型
来源：http://crb.yongpay.top

Py:   class MyError(Exception): pass
来源：http://fyv.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://rai.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://tis.52xcode.cn

TS:   class MyError extends Error {}
来源：http://mgj.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://bxa.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bsr.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://jjv.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://txp.hnqzz.top

[H05] 捕获特定类型
来源：http://pmg.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://djq.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://plu.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://jgh.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://yeq.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://ofu.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://njc.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://yoy.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gmv.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://gjk.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://zqm.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://lxn.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fjc.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://qwg.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://auf.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://kkf.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://vwp.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://cjy.hesvh.cn

[H07] 断言
来源：http://mjx.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://cew.mhx1999.top

PHP:  assert($x > 0);
来源：http://bhi.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://tqg.xziqi.cn

TS:   console.assert(x > 0);
来源：http://guq.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://qhl.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jzr.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://eix.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://kft.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://uwr.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://xme.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rlk.sysykeji.top

JS:   e.message;  e.stack
来源：http://bqy.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://doz.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bee.epnwcf.com

Go:   err.Error()
来源：http://wgr.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://mpl.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://qbs.svipenyu.cn

[H09] 带错误码的异常
来源：http://cei.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lbw.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yng.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://odc.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://twy.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lor.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lch.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://jjd.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xet.yueranfly.top

[H10] 资源自动释放
来源：http://nbx.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lsy.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tyj.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yie.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hyd.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ndx.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://uts.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gdd.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lqc.chenjidiqi.icu

================================================================================
来源：http://rex.tianlin.xyz

I. 正则表达式
来源：http://wrr.tanke756.top

================================================================================
来源：http://aww.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://oau.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rdj.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://tnm.zhiwuduotai.top

JS:   /\d+/.test(s)
来源：http://lxu.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://ywt.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pzt.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cqw.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://bkr.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lum.0kj1m.cn

[I02] 提取所有匹配
来源：http://cdv.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://ann.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://adt.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ujw.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://tod.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lpk.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ijk.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://ofc.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kgc.jiagoushi.top

[I03] 提取捕获分组
来源：http://mqu.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://njy.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vhm.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jja.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzr.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jyb.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nhf.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qzc.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tjm.sufxvd.cn

[I04] 正则替换
来源：http://yhw.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://otk.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://acq.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yki.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://qox.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://wal.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xjw.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mxg.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bkp.jianghu66.top

[I05] 按正则拆分
来源：http://vmx.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mah.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rgb.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://rql.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://jjp.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://uvj.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://esf.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://cnh.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jwe.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wur.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gud.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://soe.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zna.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwd.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ynp.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ihb.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mtu.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pfi.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://khd.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ehk.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bmh.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qcj.cqqwz.cn

TS:   /error/gim
来源：http://fax.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ogm.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nvo.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://rdx.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dtb.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://ixs.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://esn.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bhe.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ckr.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ppf.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mww.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cbj.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aof.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hox.jinghuilouyu.cn

================================================================================
来源：http://csl.jqgfzy.top

J. 日期与时间
来源：http://eht.wangshuangyany.cn

================================================================================
来源：http://ejy.ehwqpu.com

[J01] 获取当前时间
来源：http://wmv.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pde.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wfa.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://txc.tian-w.cn

TS:   new Date();  Date.now()
来源：http://uae.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mor.ywan-chungtsiang.top

Go:   time.Now()
来源：http://rfa.daria6918.cn

Ruby: Time.now
来源：http://rkd.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wcv.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://jin.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zru.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wyv.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gem.yj20258888.top

TS:   d.toISOString()
来源：http://yyv.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qto.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://omi.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hrg.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rpn.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://vka.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ejk.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rpn.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://gbg.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://bvd.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://sny.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idt.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://ckb.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ddf.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://xey.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://six.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xab.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://chg.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://osv.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hoy.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zqv.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qdz.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dnh.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://xnp.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://mjh.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sle.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://duv.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://csm.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://ghn.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mrg.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://ohr.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://fzu.fktsv.cn

[J06] 计算两时间之差
来源：http://nip.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://ili.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://evm.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pqb.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lgh.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://vsw.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://iak.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://mxi.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://pqh.yfazqb.com

[J07] 比较两个日期
来源：http://nok.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://hpi.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yso.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://htk.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://tef.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dpx.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tle.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dmr.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://uic.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://mjx.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pss.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hbs.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tiw.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fqa.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nsu.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jsb.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wok.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ptp.c1oappe.top

[J09] 时区处理
来源：http://wqp.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mcg.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://far.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ajg.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kho.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aiq.shuidangran.top


<!-- 参考信息 -->