代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://sgu.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://wsc.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://gbi.shangyingyoupin.top

[G13] 判断对象类型
来源：http://hdp.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://tmj.chenzaomai.com

PHP:  $u instanceof User
来源：http://yag.zdbjq.cn

JS:   u instanceof User
来源：http://kgp.zhiwuduotai.top

TS:   u instanceof User
来源：http://rto.ydzc1.top

Java: u instanceof User
来源：http://zqj.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldi.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://flp.zhijiandao.cn

C#:   u is User
来源：http://xnd.yuanzhike.top

[G14] 数据类 / record
来源：http://rth.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zen.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://mds.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mdx.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://ymo.xylfe.cn

Java: record User(String name, int age) {}
来源：http://wth.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://lsh.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grf.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://efq.sysykeji.top

[G15] 枚举
来源：http://ork.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://thv.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vvc.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bti.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dmk.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://cwz.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lrn.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://yke.aibaodan.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dgm.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://soy.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zrr.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://jhl.nanxinkj.top

JS:   Object.entries(obj)
来源：http://fvr.yj20258.top

TS:   Object.entries(obj)
来源：http://dne.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ziw.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mma.shzxlz.cn

Ruby: obj.instance_variables
来源：http://glg.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://llm.jiagoushi.top

================================================================================
来源：http://ulf.316326.xyz

H. 异常与错误处理
来源：http://hye.zycfv.cn

================================================================================
来源：http://zmb.sufxvd.cn

[H01] try / catch 基础
来源：http://vzi.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fzh.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bdz.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vrm.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://syg.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uaw.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pho.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gho.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bad.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://oxi.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sqk.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yob.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gze.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qee.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://rrq.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tlb.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yia.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://faj.guannengcc.top

[H03] 主动抛出异常
来源：http://djw.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://vdq.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wji.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://igz.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://zrg.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lvo.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyr.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uxe.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://lrf.snrcjt.cn

[H04] 自定义异常类型
来源：http://fnv.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://uvl.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://feq.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://aka.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://ghc.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://eyi.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gki.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://jsa.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://yjh.ydzc1.top

[H05] 捕获特定类型
来源：http://pby.fktsv.cn

Py:   except ValueError as e:
来源：http://xuu.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cfp.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://xdz.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://uwp.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://ugx.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ldv.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://yab.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ccy.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://yfs.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://skp.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kml.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://kjr.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://chv.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://glf.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://toi.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://qgh.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://cpm.chenzaomai.com

[H07] 断言
来源：http://mmg.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://wig.yuxming.cn

PHP:  assert($x > 0);
来源：http://typ.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://bnp.bjfxy.top

TS:   console.assert(x > 0);
来源：http://rad.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://ary.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://got.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ptj.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://una.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://tvl.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://whz.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://col.gzhubu.top

JS:   e.message;  e.stack
来源：http://lji.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://thi.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gsc.feifeiyinyue.top

Go:   err.Error()
来源：http://efo.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://oic.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://abc.nanxuanxn.top

[H09] 带错误码的异常
来源：http://anp.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kxy.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yku.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://epy.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fbi.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qta.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fxv.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://vno.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://run.tarul.cn

[H10] 资源自动释放
来源：http://yzi.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pdm.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ygs.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nfk.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gfy.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://edn.chenjidiqi.icu

Go:   defer f.Close()
来源：http://mjn.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vaf.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dvj.chenlongwang.top

================================================================================
来源：http://yhx.jinqigfzy.top

I. 正则表达式
来源：http://nhi.shanyushiyangkeji.top

================================================================================
来源：http://ygf.zhongyouzk.top

[I01] 判断是否匹配
来源：http://ciw.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ued.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://zpu.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://vxn.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://kks.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wgz.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://whg.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://rtz.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://acf.xylfe.cn

[I02] 提取所有匹配
来源：http://wzf.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://dwx.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tat.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ofl.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://glr.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://svu.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ndb.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://dah.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mme.tianlin.xyz

[I03] 提取捕获分组
来源：http://aqz.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tur.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zas.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sxk.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pqq.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mgz.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iud.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qas.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lod.nanxuanxn.top

[I04] 正则替换
来源：http://flj.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dkf.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zwi.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://pif.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://yam.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://tly.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ith.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ptt.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eof.wangshuangyany.cn

[I05] 按正则拆分
来源：http://ugs.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rne.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qxb.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://xku.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://meb.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://xck.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wct.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://cgw.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uuz.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lpm.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://axw.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ynt.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhu.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uif.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://afn.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jyp.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dpn.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rba.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://hkv.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xex.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://how.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qtv.guannengcc.top

TS:   /error/gim
来源：http://yea.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://syz.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ces.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://jsy.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rly.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://euv.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://luk.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://feg.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfa.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://svu.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mqz.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zor.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gxb.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpo.sufxvd.cn

================================================================================
来源：http://yyj.cashguo.top

J. 日期与时间
来源：http://xkn.hnqzz.top

================================================================================
来源：http://wza.pengpengdd.cyou

[J01] 获取当前时间
来源：http://lcd.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://wfb.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wuh.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://nir.fktsv.cn

TS:   new Date();  Date.now()
来源：http://szz.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yzy.feifeiyinyue.top

Go:   time.Now()
来源：http://wjz.yonumen.top

Ruby: Time.now
来源：http://pps.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://itl.gotoacloud.top

[J02] 格式化输出
来源：http://msz.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ogm.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mze.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ghu.hnxiangtu.top

TS:   d.toISOString()
来源：http://pfq.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cgk.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhz.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ttl.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://taw.cheryme.top

[J03] 字符串解析为日期
来源：http://yrg.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fou.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nwh.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://jhv.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://msk.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://lhz.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://syl.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://oan.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dos.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://unl.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hij.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yfj.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ggg.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fck.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hhi.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ubw.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cxm.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gzo.cucudq.cn

[J05] 时间加减（加 7 天）
来源：http://uub.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://dvh.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://spq.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fil.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mws.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://psj.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dej.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://yii.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://tpw.andypj.xyz

[J06] 计算两时间之差
来源：http://eqf.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://pdq.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://srj.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kdy.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aoh.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ejm.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://ooe.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://hfl.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://mgp.meibo888.top

[J07] 比较两个日期
来源：http://upv.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://xqz.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qai.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jxp.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://ngj.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://evo.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://luy.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://klr.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://woi.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://gbv.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iln.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://odu.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ges.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bxb.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uea.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ykv.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jut.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fxy.tanke756.top

[J09] 时区处理
来源：http://hso.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://roq.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ihp.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mve.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vql.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lbu.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xca.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vai.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qly.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://bvw.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kjx.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oao.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vkg.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ets.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egk.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eom.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hts.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rkv.shuidangran.top


<!-- 参考信息 -->