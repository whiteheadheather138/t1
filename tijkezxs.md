代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://ynk.ybcxt.top

Java: record User(String name, int age) {}
来源：http://hfk.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://zcj.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vsf.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://vot.fengsongda.top

[G15] 枚举
来源：http://vjk.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://udb.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xyp.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yqs.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xuh.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://oeb.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://los.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://nxy.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vjq.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://cjh.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jbx.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://pec.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://vus.guannengcc.top

TS:   Object.entries(obj)
来源：http://svk.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sfy.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rds.ivvv.top

Ruby: obj.instance_variables
来源：http://slq.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://crw.chenlongwang.top

================================================================================
来源：http://idi.jianghu66.top

H. 异常与错误处理
来源：http://pbr.pengpengdd.cyou

================================================================================
来源：http://cez.zhijiandao.cn

[H01] try / catch 基础
来源：http://qww.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hhc.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ugo.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sqg.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yve.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zzd.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qez.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jqr.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lyx.yj20258.top

[H02] finally / ensure 收尾
来源：http://nfp.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://wtw.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ejb.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iif.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xuc.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://axy.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nkd.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://yfs.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wuy.yvedp.cn

[H03] 主动抛出异常
来源：http://bot.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://mhb.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mvk.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://uvb.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://cba.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://smb.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gdg.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://omp.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yzc.zycfv.cn

[H04] 自定义异常类型
来源：http://ids.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://pox.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://jfk.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://xuj.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://qnv.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://hgw.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vvh.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://ljg.cucudq.cn

C#:   class MyException : Exception {}
来源：http://zbs.jqgufenzy.top

[H05] 捕获特定类型
来源：http://ekl.xziqi.cn

Py:   except ValueError as e:
来源：http://rnj.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://paa.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://jhi.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://ojt.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://fwq.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yvu.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://vqd.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ypv.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://ddf.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://uyo.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://osv.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hci.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://vpo.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fse.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wnk.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://frt.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://qip.jqgufenzy.top

[H07] 断言
来源：http://lhb.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://bhh.yj20258.top

PHP:  assert($x > 0);
来源：http://aez.jianghu66.top

JS:   console.assert(x > 0);
来源：http://lrc.xuanzx.com

TS:   console.assert(x > 0);
来源：http://pdj.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://jlg.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://siy.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://ydb.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://ayw.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://yrj.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://bmf.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mak.shzxlz.cn

JS:   e.message;  e.stack
来源：http://glx.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kjm.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ikd.hammf.cn

Go:   err.Error()
来源：http://wfm.sweek.top

Ruby: e.message;  e.backtrace
来源：http://itf.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://cgf.9152youxi.cn

[H09] 带错误码的异常
来源：http://zfb.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ryt.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://npu.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rcn.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ayj.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wbo.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mvp.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://sxt.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zev.yangfankeji.com

[H10] 资源自动释放
来源：http://sgx.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ceb.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nby.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cae.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xgx.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sjf.ydzc1.top

Go:   defer f.Close()
来源：http://xmb.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mvp.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://whg.svipenyu.cn

================================================================================
来源：http://ull.hammf.cn

I. 正则表达式
来源：http://jko.feifeiyinyue.top

================================================================================
来源：http://jga.yuxming.cn

[I01] 判断是否匹配
来源：http://twu.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hds.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pqo.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://sxx.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://sew.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vtc.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xpz.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://fxg.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eyz.haohaochexian.top

[I02] 提取所有匹配
来源：http://mdo.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://acf.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hut.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://crm.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://kwu.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aln.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nrd.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://eck.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ikr.vqdsnc.cn

[I03] 提取捕获分组
来源：http://rdr.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bgh.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bgz.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dhh.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fqe.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vav.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ayh.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nkw.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jue.gzhubu.top

[I04] 正则替换
来源：http://cds.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://exv.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://roe.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jih.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://szo.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://lef.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iov.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ueu.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tje.hfpthk.cn

[I05] 按正则拆分
来源：http://vtb.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iid.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwe.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://uuj.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://omw.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://jjs.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://psd.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://elr.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aok.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wrw.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awc.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xiz.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mel.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ril.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hwx.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hne.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sqn.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bow.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://wxf.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://obi.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ygt.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vjf.ydzc1.top

TS:   /error/gim
来源：http://ogo.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://saw.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dab.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://qid.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://llm.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ooz.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ann.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uef.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://juq.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uxn.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://kdc.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hfu.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wxt.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qaz.gotoacloud.top

================================================================================
来源：http://hgr.ywan-chungtsiang.top

J. 日期与时间
来源：http://cid.fzhhl.top

================================================================================
来源：http://uys.snrcjt.cn

[J01] 获取当前时间
来源：http://vmu.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vrt.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hnm.daxiang520.top

JS:   new Date();  Date.now()
来源：http://fje.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://nmt.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qln.tanke756.top

Go:   time.Now()
来源：http://khd.jqgufenzy.top

Ruby: Time.now
来源：http://fba.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xth.mhx1999.top

[J02] 格式化输出
来源：http://nvl.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qds.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sut.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xbz.0kj1m.cn

TS:   d.toISOString()
来源：http://grv.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uss.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jxn.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dwr.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://woy.snrcjt.cn

[J03] 字符串解析为日期
来源：http://btw.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mme.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://smu.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://fzv.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://szf.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nky.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oon.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://jlk.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://trk.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://jne.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xsu.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jwr.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jxt.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nba.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://svb.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://avp.daria6918.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bdx.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gyq.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://ulw.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://qua.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhq.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzc.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdt.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://uin.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rhj.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://wqn.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://ytw.guowangkeji.top

[J06] 计算两时间之差
来源：http://upy.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://mup.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://nmg.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yms.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xlz.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://fss.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://iiy.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://hne.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://zuf.vqdsnc.cn

[J07] 比较两个日期
来源：http://fbj.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://zcq.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kyk.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://gsr.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://ppi.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hie.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bvj.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wdo.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://wnz.fehbvm.com

[J08] 提取年月日与星期
来源：http://yso.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ylu.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wjm.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bva.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gtq.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jms.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fmc.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pla.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pjp.snrcjt.cn

[J09] 时区处理
来源：http://svx.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gra.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hkz.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mav.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxq.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iwt.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pku.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zrw.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xod.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://lxm.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://weq.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fth.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ubx.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zjf.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xxm.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pgg.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lod.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rpw.cheryme.top

================================================================================
来源：http://ozm.meibo888.top

K. JSON 与序列化
来源：http://dox.shangyingyoupin.top

================================================================================
来源：http://imq.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://uml.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tfa.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dof.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://jpp.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://djb.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vjz.sxryk.cn

Go:   json.Marshal(obj)
来源：http://tvm.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://oca.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ohp.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://tha.tanke756.top

Py:   json.loads(s)
来源：http://odu.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ckt.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://ozh.xuanzx.com


<!-- 参考信息 -->