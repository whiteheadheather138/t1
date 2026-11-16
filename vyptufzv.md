代发 wailian999

[G14] 数据类 / record
来源：http://srr.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pbh.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://wxt.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://raa.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://fkx.daria6918.cn

Java: record User(String name, int age) {}
来源：http://rgj.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://fib.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zzi.sweek.top

C#:   record User(string Name, int Age);
来源：http://uyu.fengsongda.top

[G15] 枚举
来源：http://iuj.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blo.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vvj.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ymn.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mvf.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://xfv.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dsw.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://lkl.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nxo.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://zkv.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aib.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://tkt.yuxming.cn

JS:   Object.entries(obj)
来源：http://red.tarul.cn

TS:   Object.entries(obj)
来源：http://sjl.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zll.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://evl.gzhubu.top

Ruby: obj.instance_variables
来源：http://huc.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://cyl.xinyue.icu

================================================================================
来源：http://epv.shuidangran.top

H. 异常与错误处理
来源：http://knw.sufxvd.cn

================================================================================
来源：http://byl.xziqi.cn

[H01] try / catch 基础
来源：http://nep.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://olv.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zww.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jov.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gvs.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tij.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sjf.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wsf.jianghu66.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pur.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://sup.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jrk.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kct.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://irm.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lyl.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://auc.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rfw.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gir.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eio.tanke756.top

[H03] 主动抛出异常
来源：http://gop.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://dol.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ihr.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://quj.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://jqv.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://coi.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mbx.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sty.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gzt.xylfe.cn

[H04] 自定义异常类型
来源：http://ddi.cashguo.top

Py:   class MyError(Exception): pass
来源：http://ncx.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://asv.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://dnb.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://wzi.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://krp.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kuj.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://def.vehdjk.com

C#:   class MyException : Exception {}
来源：http://rec.fktsv.cn

[H05] 捕获特定类型
来源：http://qvn.gotoacloud.top

Py:   except ValueError as e:
来源：http://tck.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lwc.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://siq.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://jnu.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://ctz.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xiq.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://gln.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gel.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://mbc.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://cxg.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nuc.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://yai.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cnv.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ujm.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wgy.yanxiufei.cn

Ruby: d&.dig(:a, :b)
来源：http://dsj.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://eoz.ivvv.top

[H07] 断言
来源：http://izu.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://nqv.dashuyun.cn

PHP:  assert($x > 0);
来源：http://pes.xinyue.icu

JS:   console.assert(x > 0);
来源：http://nnu.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://vfh.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://wnz.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uuc.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://rdb.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://dyp.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://ftw.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://wly.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kye.bjfxy.top

JS:   e.message;  e.stack
来源：http://tav.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tsq.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cls.jqgufenzy.top

Go:   err.Error()
来源：http://lmc.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://yrj.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://evw.fengsongda.top

[H09] 带错误码的异常
来源：http://szb.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://twv.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bou.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cew.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yxs.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dmz.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://siv.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://prf.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ptm.chenzaomai.com

[H10] 资源自动释放
来源：http://bje.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gxj.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nrw.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://apz.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ywq.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://llt.zdqjudy.top

Go:   defer f.Close()
来源：http://drr.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bit.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://faj.fehbvm.com

================================================================================
来源：http://vix.yvedp.cn

I. 正则表达式
来源：http://rok.gzhubu.top

================================================================================
来源：http://fwb.jinqigufen.top

[I01] 判断是否匹配
来源：http://pyu.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://anm.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://wtp.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://njw.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://lwr.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bai.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oth.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://zrv.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dnr.redwolf501.top

[I02] 提取所有匹配
来源：http://cmt.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://xny.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pgg.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pen.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://ufy.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rct.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eef.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://mij.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lfm.0kj1m.cn

[I03] 提取捕获分组
来源：http://tfl.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://prz.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://awo.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nmt.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qbo.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ujp.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fdz.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://puw.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yhh.zhoulong.xyz

[I04] 正则替换
来源：http://hbt.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://daa.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fpm.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kuo.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://kpv.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://aaq.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qta.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://aam.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://goz.vqdsnc.cn

[I05] 按正则拆分
来源：http://rgr.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xir.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dce.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://nzk.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://jzt.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://gvj.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dwl.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fxq.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xyj.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hbp.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xqg.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://prn.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rgh.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lef.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wvb.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hxk.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mbc.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cmd.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://nmt.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yhn.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sbr.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pbd.yj202588.top

TS:   /error/gim
来源：http://kkw.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nlp.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fkz.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://kyf.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://son.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://guk.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://syg.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wai.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ftu.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://egq.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lwq.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bgz.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://old.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fle.dianchejie.cn

================================================================================
来源：http://tlk.gzhubu.top

J. 日期与时间
来源：http://gwy.wangshuangyany.cn

================================================================================
来源：http://mff.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://kns.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wjm.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gtf.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://umn.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://frd.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iei.wangshuangyany.cn

Go:   time.Now()
来源：http://oag.mhx1999.top

Ruby: Time.now
来源：http://ojw.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://npv.jqgufenzy.top

[J02] 格式化输出
来源：http://plt.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xrc.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jlg.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kzz.daria6918.cn

TS:   d.toISOString()
来源：http://qqx.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hpw.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vyj.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ybo.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://svk.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://ilw.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyq.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpm.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://yem.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://qbb.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://fxp.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lqb.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://wut.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jfi.bjfxy.top

[J04] 时间戳与日期互转
来源：http://qmp.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yar.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nro.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lnz.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cxx.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xaa.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hyu.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kzm.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pik.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://zlu.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://ags.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uad.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xxq.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hdd.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://ysg.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fww.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://jke.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://tmz.gzhubu.top

[J06] 计算两时间之差
来源：http://gux.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://ozk.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://qph.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gnv.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dny.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://xgw.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://wqm.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://rsb.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://qkt.gogol.net.cn

[J07] 比较两个日期
来源：http://mhx.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://pqy.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cvu.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dim.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://okl.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qab.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://skj.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sew.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://efs.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://zxf.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://atm.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ivn.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hfl.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pxu.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cnp.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://enp.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://etm.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://klh.wangshuangyany.cn

[J09] 时区处理
来源：http://uid.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cah.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ini.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ijr.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kld.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ydy.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwo.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://llt.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lvx.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://cxh.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://quf.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uzj.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vby.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ksk.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://leg.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kzs.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kzy.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qgm.sufxvd.cn

================================================================================
来源：http://uqn.hysaishi.cn

K. JSON 与序列化
来源：http://zth.wangdashe.top

================================================================================
来源：http://wfv.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://cto.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mep.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wvm.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://qif.cashguo.top

TS:   JSON.stringify(obj)
来源：http://zaa.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ncu.pycfn.com

Go:   json.Marshal(obj)
来源：http://rno.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rjo.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xru.chenlongwang.top


<!-- 参考信息 -->