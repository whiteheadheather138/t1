代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://gdn.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://pfn.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://ton.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://adp.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://mpz.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://gmi.yj20258.top

C#:   public override string ToString() => Name;
来源：http://tjm.nanxinkj.top

[G13] 判断对象类型
来源：http://gth.fzhhl.top

Py:   isinstance(u, User)
来源：http://ugy.gaohongyu789.top

PHP:  $u instanceof User
来源：http://scu.chenlongwang.top

JS:   u instanceof User
来源：http://feb.bbcook.cn

TS:   u instanceof User
来源：http://asl.jqgfzy.top

Java: u instanceof User
来源：http://vme.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zrj.yuxming.cn

Ruby: u.is_a?(User)
来源：http://ltc.vehdjk.com

C#:   u is User
来源：http://dsn.hcnkem.com

[G14] 数据类 / record
来源：http://ewf.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wid.9152youxi.cn

PHP:  // 用 readonly 属性模拟
来源：http://wcq.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://clp.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://aee.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://xrv.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://eun.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hxw.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://cur.gzhubu.top

[G15] 枚举
来源：http://ipt.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mzr.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xyu.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dja.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://apb.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://sdl.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qyz.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://ygx.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vwr.smart0.xyz

[G16] 对象转数组 / 字典
来源：http://bpz.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cor.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://zqp.cucudq.cn

JS:   Object.entries(obj)
来源：http://jab.daxiang520.top

TS:   Object.entries(obj)
来源：http://uzc.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ubk.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://axu.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://unt.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://pbe.cucudq.cn

================================================================================
来源：http://dvz.bbcook.cn

H. 异常与错误处理
来源：http://mlo.nwbrower.top

================================================================================
来源：http://gew.chenzaomai.com

[H01] try / catch 基础
来源：http://rlg.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rxx.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xbs.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vda.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iqh.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ybr.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ovl.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://snj.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://umw.fehbvm.com

[H02] finally / ensure 收尾
来源：http://dkx.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://mgq.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cxk.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cif.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mxd.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://nwr.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qea.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://vol.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nfv.yuxming.cn

[H03] 主动抛出异常
来源：http://grs.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://hyc.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jyr.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://zve.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://urk.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rlm.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ksx.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uyj.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://kmb.zdbjq.cn

[H04] 自定义异常类型
来源：http://hyh.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://pnj.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xxm.yj20258.top

JS:   class MyError extends Error {}
来源：http://ohf.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://hqn.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://xvn.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gpr.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://xcj.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://aig.wangdashe.top

[H05] 捕获特定类型
来源：http://swj.sufxvd.cn

Py:   except ValueError as e:
来源：http://fuv.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wvy.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://eni.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://wpi.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://eyr.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xcd.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://jnx.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zzy.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://jta.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://see.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rxk.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cpc.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://ofu.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ktg.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ned.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://zsk.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://egv.ctjpmb.com

[H07] 断言
来源：http://eiq.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://bii.bjfxy.top

PHP:  assert($x > 0);
来源：http://wdi.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://tpg.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://aus.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://iug.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yue.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://dtj.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://mhw.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://cep.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://uch.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sra.hywenlv.cn

JS:   e.message;  e.stack
来源：http://cbj.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dfi.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ypm.aibaodan.cn

Go:   err.Error()
来源：http://llp.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://yov.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://zxo.guannengcc.top

[H09] 带错误码的异常
来源：http://mlj.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mgr.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://zxi.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bmp.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kkk.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cwj.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tfi.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://gyk.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ipk.vqdsnc.cn

[H10] 资源自动释放
来源：http://jxu.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ptd.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zol.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jff.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cyc.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qgr.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://rbn.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zbq.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zta.9152youxi.cn

================================================================================
来源：http://hnk.sweek.top

I. 正则表达式
来源：http://lga.yonumen.top

================================================================================
来源：http://phk.9152youxi.cn

[I01] 判断是否匹配
来源：http://aiv.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oej.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://uvg.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://tnb.yfazqb.com

TS:   /\d+/.test(s)
来源：http://fod.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://whf.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ufi.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://caj.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xqa.ppjwa.cn

[I02] 提取所有匹配
来源：http://ayh.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://cqe.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://noj.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lsr.hammf.cn

TS:   s.match(/\d+/g)
来源：http://rdw.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jkl.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wff.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://qxf.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ler.wangdashe.top

[I03] 提取捕获分组
来源：http://las.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cof.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yss.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gzj.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pbd.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ypk.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yef.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://glg.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://akz.daria6918.cn

[I04] 正则替换
来源：http://vsb.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://jgo.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lwg.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://yrt.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://gwb.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yor.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://qau.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tiq.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cns.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://iqv.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ulv.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hvx.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://hes.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://wqu.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://euv.meibo888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jao.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ict.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ejk.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ovl.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ess.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://szf.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://keq.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ozc.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ogc.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fne.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gnu.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ldi.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://cqc.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xis.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nhn.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vzf.dashuyun.cn

TS:   /error/gim
来源：http://ptj.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tgd.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nrn.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://rtx.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ntd.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://hhd.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bqh.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eam.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://snf.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pew.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nik.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bww.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aea.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tmm.nanxuanxn.top

================================================================================
来源：http://neh.zhaomingkeji.xyz

J. 日期与时间
来源：http://aqb.ydzc1.top

================================================================================
来源：http://cnm.ivvv.top

[J01] 获取当前时间
来源：http://iwi.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xsm.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pwc.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://xch.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://rtn.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lzn.gogol.net.cn

Go:   time.Now()
来源：http://hyd.meibo888.top

Ruby: Time.now
来源：http://pcb.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nfq.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://bxc.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://usz.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ztn.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nwu.mhx1999.top

TS:   d.toISOString()
来源：http://ttz.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mir.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ojy.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfy.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fos.yj202588.top

[J03] 字符串解析为日期
来源：http://dma.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kjp.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lbd.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://alv.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://gke.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pvf.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rat.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://bif.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://djq.birdmap.top

[J04] 时间戳与日期互转
来源：http://zyj.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ijq.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ewm.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tuq.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cem.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rtu.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vch.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pnq.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mgi.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://pch.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://spo.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://red.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddg.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://auc.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://fsk.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ran.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://nkf.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://fcy.ppjwa.cn

[J06] 计算两时间之差
来源：http://nco.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://sus.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://gbd.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xes.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xtj.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://zco.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://tnm.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://jkg.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://spt.shuidangran.top

[J07] 比较两个日期
来源：http://oag.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://xfq.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jts.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jdy.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pje.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rln.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kan.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://idp.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://bwe.ybcxt.top

[J08] 提取年月日与星期
来源：http://rxg.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sny.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xxy.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jcx.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://unz.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gqc.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vto.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gqz.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hzh.xylfe.cn

[J09] 时区处理
来源：http://grt.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://voz.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhp.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uul.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kyn.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sys.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ays.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tnz.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gty.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://abf.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://skr.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://alt.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://obf.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://daq.fktsv.cn


<!-- 参考信息 -->