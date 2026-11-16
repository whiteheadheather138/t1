代发 wailian999

Py:   isinstance(u, User)
来源：http://ywx.jianghu66.top

PHP:  $u instanceof User
来源：http://rot.nanxinkj.top

JS:   u instanceof User
来源：http://nwj.kuanghao11.cn

TS:   u instanceof User
来源：http://hmu.jiagoushi.top

Java: u instanceof User
来源：http://kal.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://czf.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://zdg.yongpay.top

C#:   u is User
来源：http://tjx.xziqi.cn

[G14] 数据类 / record
来源：http://ysm.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nfl.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://wxd.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://oze.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://yvm.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://lxt.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://mtc.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tga.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://csq.fzhhl.top

[G15] 枚举
来源：http://ago.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zdx.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://gcb.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fxd.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://usw.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://jmt.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jpq.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://gzb.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nfg.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://vnk.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ywn.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://adx.hfpthk.cn

JS:   Object.entries(obj)
来源：http://nhe.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://fjd.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xca.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://brv.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://jvp.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://sbu.chenlongwang.top

================================================================================
来源：http://axz.ybcxt.top

H. 异常与错误处理
来源：http://gnr.nwbrower.top

================================================================================
来源：http://rgh.nanxuanxn.top

[H01] try / catch 基础
来源：http://jga.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iak.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ejj.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uza.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zzk.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jyx.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cwt.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bla.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rkl.ybcxt.top

[H02] finally / ensure 收尾
来源：http://nlc.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fhi.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://usg.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aen.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://kro.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://dqw.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fbs.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://uck.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wew.nanxinkj.top

[H03] 主动抛出异常
来源：http://rjc.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://btk.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bdl.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://mts.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://hwl.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ggl.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://not.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://pxg.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dih.ehwqpu.com

[H04] 自定义异常类型
来源：http://ryl.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://yru.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://rmg.daxiang520.top

JS:   class MyError extends Error {}
来源：http://obw.316326.xyz

TS:   class MyError extends Error {}
来源：http://tha.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://uqs.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aie.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://awg.shuidangran.top

C#:   class MyException : Exception {}
来源：http://qdt.jqgufenzy.top

[H05] 捕获特定类型
来源：http://jqo.mhx1999.top

Py:   except ValueError as e:
来源：http://wos.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ohh.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://mjy.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://qoi.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://ubn.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lla.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://zto.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://geg.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://kml.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://pti.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://kak.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://xyr.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aaz.havefunace.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rjv.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fry.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://qpl.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://ggm.pengpengdd.cyou

[H07] 断言
来源：http://bsp.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://xgu.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://lym.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://nzt.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://fub.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://mkm.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hgz.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://sab.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://xxs.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://ony.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://ias.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://szc.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://cpu.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfp.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rko.tianlin.xyz

Go:   err.Error()
来源：http://ckz.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://pwj.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://oli.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://ofr.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ybr.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oyu.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wdr.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://spy.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gxf.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lli.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jzn.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://crn.jinqigufen.top

[H10] 资源自动释放
来源：http://qdv.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lke.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jos.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mqc.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ucy.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ran.yanxiufei.cn

Go:   defer f.Close()
来源：http://obz.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nkn.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ulh.cheryme.top

================================================================================
来源：http://abh.hnqzz.top

I. 正则表达式
来源：http://unk.jqgfzy.top

================================================================================
来源：http://giu.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://gdf.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hsb.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://tof.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://xay.guannengcc.top

TS:   /\d+/.test(s)
来源：http://ext.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xnb.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hgs.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://mwk.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://orz.fengsongda.top

[I02] 提取所有匹配
来源：http://wgs.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://suz.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qjh.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://emz.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://zis.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://siw.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dom.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://nzl.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bqw.jqgufenzy.top

[I03] 提取捕获分组
来源：http://ura.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mdn.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vqx.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rnn.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://byk.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tkp.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nvf.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://onu.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://upz.jinqigfzy.top

[I04] 正则替换
来源：http://edt.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mon.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vmw.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://oes.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://wcq.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mzm.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ceo.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ktf.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hzo.svipenyu.cn

[I05] 按正则拆分
来源：http://mlb.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://ohx.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gdq.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://azl.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://zkl.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://kvd.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ocy.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://dml.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vvm.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://czz.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gwk.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tvk.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bif.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krj.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hap.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hqx.sweek.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qqw.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ccq.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://hlz.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iba.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ycc.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ndy.pengpengdd.cyou

TS:   /error/gim
来源：http://qac.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fpb.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://puh.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://yzi.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tiz.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://xkj.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xsf.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://izy.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dle.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wjk.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sre.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mgh.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wwf.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wqm.svipenyu.cn

================================================================================
来源：http://seg.yuanzhike.top

J. 日期与时间
来源：http://ebo.chenlongwang.top

================================================================================
来源：http://vos.guowangkeji.top

[J01] 获取当前时间
来源：http://rgm.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://khv.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwr.yonumen.top

JS:   new Date();  Date.now()
来源：http://qsk.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://twv.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yry.meibo888.top

Go:   time.Now()
来源：http://esu.jlsjyb.cn

Ruby: Time.now
来源：http://fmz.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://efl.jinqigufen.top

[J02] 格式化输出
来源：http://voz.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gsh.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lap.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jtc.feifeiyinyue.top

TS:   d.toISOString()
来源：http://yju.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hpt.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xib.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cgs.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fgd.aibaodan.cn

[J03] 字符串解析为日期
来源：http://weh.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vwf.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gtr.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://fsy.yonumen.top

TS:   new Date("2024-01-02")
来源：http://cmi.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://xec.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oad.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://uue.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kny.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://lli.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eui.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xtc.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://azq.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eit.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tak.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zcq.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xqz.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://glg.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://irq.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://zko.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cml.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bkt.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ukf.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://fke.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mwm.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://qqh.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wmg.aizwys.cn

[J06] 计算两时间之差
来源：http://fol.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://zam.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://rvx.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lzi.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cll.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://ffa.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://ttm.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://ltn.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://pjt.gogol.net.cn

[J07] 比较两个日期
来源：http://plp.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://sba.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ufn.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://fkk.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://qjf.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pbg.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://unu.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://jxx.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://tse.sysykeji.top

[J08] 提取年月日与星期
来源：http://wcr.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qqx.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gbk.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vmj.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://imv.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://brz.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iyk.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vgj.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cfk.yj20258888.top

[J09] 时区处理
来源：http://wal.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dbk.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://drp.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zuf.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rbg.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://syg.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bwi.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bft.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ldx.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://tus.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fog.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gmx.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://osv.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tev.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jcf.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uyf.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ljf.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://exg.yj20258888.top

================================================================================
来源：http://bul.daria6918.cn

K. JSON 与序列化
来源：http://avx.dashuyun.cn

================================================================================
来源：http://mtk.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://npt.xinyue.icu


<!-- 参考信息 -->