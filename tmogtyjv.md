代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://kfw.daria6918.cn

Java: record User(String name, int age) {}
来源：http://cag.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://ncq.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gbh.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://hpj.meibo888.top

[G15] 枚举
来源：http://kjb.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qtv.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tdh.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ovg.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uje.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://cds.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ade.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://mnk.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cmg.tanke756.top

[G16] 对象转数组 / 字典
来源：http://krl.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wdz.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://zsq.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://hvr.cheryme.top

TS:   Object.entries(obj)
来源：http://kgj.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hjd.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oof.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://qrq.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://ett.pycfn.com

================================================================================
来源：http://eet.ydjk.org.cn

H. 异常与错误处理
来源：http://vvt.zycfv.cn

================================================================================
来源：http://lnn.yuxming.cn

[H01] try / catch 基础
来源：http://czd.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bbf.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uvf.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sil.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qki.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ren.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://abh.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sjk.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://axk.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://kqm.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vay.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://wgg.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gwi.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://sgq.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://poa.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xoc.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dao.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sls.svipenyu.cn

[H03] 主动抛出异常
来源：http://stg.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://tqm.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ydl.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://phm.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://pyp.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xhe.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gsc.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gdp.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://nom.fengsongda.top

[H04] 自定义异常类型
来源：http://myy.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://oep.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://esa.hammf.cn

JS:   class MyError extends Error {}
来源：http://dou.xziqi.cn

TS:   class MyError extends Error {}
来源：http://zzx.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://pmj.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gmi.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://rgq.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://der.hnxiangtu.top

[H05] 捕获特定类型
来源：http://vyh.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://mvi.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kqc.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://vfy.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://hax.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://our.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ycw.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://njf.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ool.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://hbc.shuidangran.top

Py:   value = d.get("k") or default
来源：http://ffl.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hwb.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://zrs.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://vlx.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xrj.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kcy.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://quh.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://rvx.tian-w.cn

[H07] 断言
来源：http://ekm.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://dce.shzxlz.cn

PHP:  assert($x > 0);
来源：http://vaj.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://aja.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://zsd.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://kjk.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://spy.jiagoushi.top

Ruby: raise "必须为正" unless x > 0
来源：http://osu.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://jde.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://hwh.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://ski.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ioe.yvedp.cn

JS:   e.message;  e.stack
来源：http://kbr.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ebg.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pof.dianchejie.cn

Go:   err.Error()
来源：http://yvk.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://bub.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://orm.dashuyun.cn

[H09] 带错误码的异常
来源：http://vwq.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ezf.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jal.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pnt.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tqy.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ggq.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hjy.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ara.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://als.haohaochexian.top

[H10] 资源自动释放
来源：http://pbx.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vtt.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://njn.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://giw.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vdt.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://owv.bjfxy.top

Go:   defer f.Close()
来源：http://ulu.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://usp.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sia.ctjpmb.com

================================================================================
来源：http://wsx.zhiwuduotai.top

I. 正则表达式
来源：http://vkd.hysaishi.cn

================================================================================
来源：http://sfk.redwolf501.top

[I01] 判断是否匹配
来源：http://hob.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pgw.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://wid.ybcxt.top

JS:   /\d+/.test(s)
来源：http://trs.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://dsp.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://llb.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sxh.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://loh.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lgd.bjfxy.top

[I02] 提取所有匹配
来源：http://gsb.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://wwx.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yea.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vlm.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://lvj.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lae.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ihw.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://rru.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ynx.nanxuanxn.top

[I03] 提取捕获分组
来源：http://ztd.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fnl.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zbd.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zri.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xqd.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://clz.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fry.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qka.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://taa.shanyushiyangtech.top

[I04] 正则替换
来源：http://lht.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dtb.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uss.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://ati.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://iki.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://hbt.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hfh.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iug.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kbk.cdnleiting.top

[I05] 按正则拆分
来源：http://see.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vhn.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mpk.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://hyl.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://mni.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://idb.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lra.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://tyt.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ncl.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lfp.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ghe.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxa.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yml.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ryq.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kmd.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aym.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kxl.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uyc.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://ekz.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fog.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jxb.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lxx.xuetiantiany.cn

TS:   /error/gim
来源：http://nus.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zhb.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dnd.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://uqp.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://suf.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://agb.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ukg.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pyu.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tkd.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ipt.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ldn.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bio.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ohi.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tcz.yonumen.top

================================================================================
来源：http://cbd.yongpay.top

J. 日期与时间
来源：http://omc.yanxiufei.cn

================================================================================
来源：http://vlr.nwbrower.top

[J01] 获取当前时间
来源：http://uat.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://msm.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kem.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://mos.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://xbd.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bbd.nanxuanxn.top

Go:   time.Now()
来源：http://qlw.haohaochexian.top

Ruby: Time.now
来源：http://ubp.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zyu.sjlbkw.cn

[J02] 格式化输出
来源：http://wje.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://znu.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tsx.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zag.nwbrower.top

TS:   d.toISOString()
来源：http://klk.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rpm.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wtm.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zze.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gsm.pycfn.com

[J03] 字符串解析为日期
来源：http://iqx.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yoz.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://duj.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://hhd.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://jfv.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ulq.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yvt.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://mls.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sdw.birdmap.top

[J04] 时间戳与日期互转
来源：http://ygz.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dmc.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ppb.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qwr.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://cno.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xcp.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hyp.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wbo.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yqw.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://plf.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://gez.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ave.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qqb.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iga.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://hlk.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zoh.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://cnl.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://gib.guowangkeji.top

[J06] 计算两时间之差
来源：http://sgc.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://pyh.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://wfg.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pgn.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uov.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kou.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://nnz.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://yfh.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://kaw.guannengcc.top

[J07] 比较两个日期
来源：http://fno.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://zqs.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kxb.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uxi.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://arv.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wsv.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yhr.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://mdq.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://apx.pycfn.com

[J08] 提取年月日与星期
来源：http://qev.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ypz.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wit.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uno.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ckm.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yew.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lhu.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qhy.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xub.zycfv.cn

[J09] 时区处理
来源：http://jlx.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ktu.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tau.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqb.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzr.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qix.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oqn.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gha.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://unm.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://nec.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wgx.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dil.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wdr.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pnk.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hlp.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ikl.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bwa.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://swj.jqgfzy.top

================================================================================
来源：http://qit.xziqi.cn

K. JSON 与序列化
来源：http://swt.zdqjudy.top

================================================================================
来源：http://enc.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://orf.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vho.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tqs.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://wfb.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://lee.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yfj.sweek.top

Go:   json.Marshal(obj)
来源：http://yeo.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://myv.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tvl.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://opc.bbcook.cn

Py:   json.loads(s)
来源：http://ifl.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bau.bjfxy.top

JS:   JSON.parse(s)
来源：http://aki.cheryme.top


<!-- 参考信息 -->