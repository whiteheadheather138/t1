代发 wailian999

Ruby: attr_accessor :name
来源：http://rvv.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://jbf.redwolf501.top

[G12] 对象转字符串
来源：http://zql.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://koz.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hpi.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://zxa.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://kcg.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://pbj.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vms.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://jst.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://zbe.52xcode.cn

[G13] 判断对象类型
来源：http://dcu.hcnkem.com

Py:   isinstance(u, User)
来源：http://xlg.xinyue.icu

PHP:  $u instanceof User
来源：http://nqy.nanxinkj.top

JS:   u instanceof User
来源：http://ukv.mhx1999.top

TS:   u instanceof User
来源：http://mwg.epnwcf.com

Java: u instanceof User
来源：http://csm.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ypw.birdmap.top

Ruby: u.is_a?(User)
来源：http://vtc.jinyuanbaomall.cn

C#:   u is User
来源：http://fvx.gaohongyu789.top

[G14] 数据类 / record
来源：http://ghq.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fko.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://vpm.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://xij.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://csl.iojbl.cn

Java: record User(String name, int age) {}
来源：http://dss.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://fxg.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kou.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://uzy.bbcook.cn

[G15] 枚举
来源：http://hac.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ndh.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wsh.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qfr.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pip.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://kdp.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cpm.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://bdw.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kdc.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://hgg.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ugh.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://qls.daria6918.cn

JS:   Object.entries(obj)
来源：http://rvy.jiagoushi.top

TS:   Object.entries(obj)
来源：http://ryb.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sct.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bdz.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://wab.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pvn.andypj.xyz

================================================================================
来源：http://jdw.snrcjt.cn

H. 异常与错误处理
来源：http://tgg.yj20258.top

================================================================================
来源：http://hlh.bbcook.cn

[H01] try / catch 基础
来源：http://lsr.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xfm.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hkt.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dbl.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sod.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fzt.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wjl.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xgy.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://epk.sxryk.cn

[H02] finally / ensure 收尾
来源：http://zlq.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://pis.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://oqp.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://psq.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yni.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zey.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mqa.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oza.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vee.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://azn.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://bxe.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tlp.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://del.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://osr.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hge.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mvs.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://cdw.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eua.zycfv.cn

[H04] 自定义异常类型
来源：http://tou.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://nzp.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://uek.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://fnz.ivvv.top

TS:   class MyError extends Error {}
来源：http://xdh.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://wjs.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bed.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://aij.ydzc1.top

C#:   class MyException : Exception {}
来源：http://eac.yuxming.cn

[H05] 捕获特定类型
来源：http://iwf.sxryk.cn

Py:   except ValueError as e:
来源：http://tnr.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uya.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://iyg.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://zrn.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://gqw.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://osw.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://ndv.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lgk.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://goh.sxryk.cn

Py:   value = d.get("k") or default
来源：http://ern.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xsk.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wtn.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vwl.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://car.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dli.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://jfl.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://fgu.sufxvd.cn

[H07] 断言
来源：http://rpn.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://nho.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://lfx.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://gzu.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://azx.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://nqe.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://spm.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://cya.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://pbw.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://xgr.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://xzp.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zvu.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://ajm.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fox.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://paz.guannengcc.top

Go:   err.Error()
来源：http://uax.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://eik.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://rld.yanxiufei.cn

[H09] 带错误码的异常
来源：http://asn.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kif.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mot.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jme.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sqp.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jkb.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jdv.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://dlk.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ylk.gzhubu.top

[H10] 资源自动释放
来源：http://yrp.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://pyn.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xkn.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://miu.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zip.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dzv.kuanghao11.cn

Go:   defer f.Close()
来源：http://jyz.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dqd.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vyp.zhongyouzk.top

================================================================================
来源：http://knx.xuetiantiany.cn

I. 正则表达式
来源：http://ldv.ppjwa.cn

================================================================================
来源：http://zak.yonumen.top

[I01] 判断是否匹配
来源：http://nct.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cps.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://jov.nwbrower.top

JS:   /\d+/.test(s)
来源：http://zcp.hcnkem.com

TS:   /\d+/.test(s)
来源：http://aze.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nqx.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bip.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://rtc.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nis.hesvh.cn

[I02] 提取所有匹配
来源：http://axy.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://feh.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hev.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ikm.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://uez.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mox.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://goc.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://oin.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ljl.hysaishi.cn

[I03] 提取捕获分组
来源：http://ivj.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lca.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ckd.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fxb.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sby.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uat.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yiu.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aqs.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jjv.sjlbkw.cn

[I04] 正则替换
来源：http://oci.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tyj.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xyo.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qel.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://ycq.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kwr.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ilv.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vlx.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ynh.xuanzx.com

[I05] 按正则拆分
来源：http://kei.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lhg.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tlg.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://akq.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://eqz.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://ahx.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oah.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://ern.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tav.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ozv.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rrq.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xim.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://duy.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwq.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kso.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oqz.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pam.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ycy.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://lyo.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bxb.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgt.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cxh.hcnkem.com

TS:   /error/gim
来源：http://yak.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rle.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eyj.meibo888.top

Ruby: s.scan(/error/i)
来源：http://izv.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vcy.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://kvb.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rqp.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mqy.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ifo.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rvd.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://blw.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://maa.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pvd.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gjg.zhoulong.xyz

================================================================================
来源：http://tcv.fzhhl.top

J. 日期与时间
来源：http://maj.zhijiandao.cn

================================================================================
来源：http://omh.jinqigfzy.top

[J01] 获取当前时间
来源：http://ayy.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nlq.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cmr.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://xru.epnwcf.com

TS:   new Date();  Date.now()
来源：http://huh.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fll.cqqwz.cn

Go:   time.Now()
来源：http://ebx.yj202588.top

Ruby: Time.now
来源：http://opt.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qop.jyoumei.cn

[J02] 格式化输出
来源：http://dsg.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xex.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dqy.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://geu.xylfe.cn

TS:   d.toISOString()
来源：http://pvw.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dhe.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tiw.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gik.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://juv.fzhhl.top

[J03] 字符串解析为日期
来源：http://ukq.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vwz.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sya.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://fwe.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://dun.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ocd.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://snn.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://vqi.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bvc.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://ijd.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vst.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hcz.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsr.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dnd.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nyh.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ipu.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uga.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nsa.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://xea.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://utp.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fwp.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ylp.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vca.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://uxi.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ftu.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://ljn.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://bng.andypj.xyz

[J06] 计算两时间之差
来源：http://uek.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://etu.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://osd.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://prc.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://img.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://gzp.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://tzl.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://jle.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://vzq.sxryk.cn

[J07] 比较两个日期
来源：http://nfq.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://gwp.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nwq.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fqk.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://jtz.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wci.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://anw.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wix.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ypb.hammf.cn

[J08] 提取年月日与星期
来源：http://med.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://foz.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vos.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gpe.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://der.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ouc.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bhu.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gkj.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://flv.redwolf501.top

[J09] 时区处理
来源：http://uvy.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://imq.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qhx.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iwu.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mty.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bbt.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lrh.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fou.sufxvd.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://scq.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://iha.jqgfzy.top


<!-- 参考信息 -->