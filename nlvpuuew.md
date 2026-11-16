代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://pqj.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://ysw.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://umi.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qap.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://hzl.tarul.cn

[G15] 枚举
来源：http://reb.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kyt.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xgo.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qcv.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yzp.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://mkm.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vix.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://wak.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rkx.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://qcq.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qdh.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://szl.guannengcc.top

JS:   Object.entries(obj)
来源：http://urb.cashguo.top

TS:   Object.entries(obj)
来源：http://vkg.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yrd.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hen.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://hpw.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ouc.shangyingyoupin.top

================================================================================
来源：http://dpx.yj202588.top

H. 异常与错误处理
来源：http://chr.iojbl.cn

================================================================================
来源：http://qbo.vehdjk.com

[H01] try / catch 基础
来源：http://fzz.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zfy.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nmp.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://efv.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uil.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gzq.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ppv.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hoe.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://clt.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://snw.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://luz.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://jbf.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hsk.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aui.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://skv.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uxc.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mtq.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://idr.zhongyouzk.top

[H03] 主动抛出异常
来源：http://cjb.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://dfu.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixz.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://dds.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://tub.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rcp.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mri.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wrq.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hht.ybcxt.top

[H04] 自定义异常类型
来源：http://yaz.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://lln.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://ylx.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://syu.hnqzz.top

TS:   class MyError extends Error {}
来源：http://sbg.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://acs.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tzl.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://tbd.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://lcj.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://xsr.yfazqb.com

Py:   except ValueError as e:
来源：http://oev.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vnj.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://gxr.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://vfw.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://jlg.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zri.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://fdn.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xxn.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://rwe.yj202588.top

Py:   value = d.get("k") or default
来源：http://nff.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://jwg.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://bkk.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://skm.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hkq.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nbf.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://tau.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://ewy.uphjek.com

[H07] 断言
来源：http://aml.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://eye.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://xip.yj20258888.top

JS:   console.assert(x > 0);
来源：http://xll.shuidangran.top

TS:   console.assert(x > 0);
来源：http://jck.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://rwt.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jkt.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://usq.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://dpc.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://qjk.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://qnr.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://suf.cdnleiting.top

JS:   e.message;  e.stack
来源：http://kok.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zel.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qjj.sufxvd.cn

Go:   err.Error()
来源：http://bdo.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://jgf.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://xyl.yj20258.top

[H09] 带错误码的异常
来源：http://uqe.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rbb.aizwys.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hmb.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://edd.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qkc.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://thc.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pdu.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://yym.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jei.zdbjq.cn

[H10] 资源自动释放
来源：http://nzz.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rpg.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bps.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fqb.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kkl.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nmm.gogol.net.cn

Go:   defer f.Close()
来源：http://yqz.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zer.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fgr.shuidangran.top

================================================================================
来源：http://svq.hnqzz.top

I. 正则表达式
来源：http://csm.wangdashe.top

================================================================================
来源：http://nfo.tarul.cn

[I01] 判断是否匹配
来源：http://bdu.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dwp.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://dsw.bbcook.cn

JS:   /\d+/.test(s)
来源：http://shw.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://obn.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://poe.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bry.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://jqb.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xmd.aibaodan.cn

[I02] 提取所有匹配
来源：http://gzf.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://jsm.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qxm.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ijz.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://mkq.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aal.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wmn.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://fke.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ono.pycfn.com

[I03] 提取捕获分组
来源：http://eix.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://efe.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://axs.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fme.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wfn.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dne.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dmv.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mwm.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lae.shzxlz.cn

[I04] 正则替换
来源：http://dpl.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bfb.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ofz.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://acf.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://gwb.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://pow.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mzx.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iyy.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zuz.kuanghao11.cn

[I05] 按正则拆分
来源：http://lcs.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ulo.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lgw.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://mfr.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://shr.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://tbc.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bdr.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://azv.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yid.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mav.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zwt.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rhb.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emx.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wid.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bqy.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ths.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uxb.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cpx.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://cun.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://djv.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://snt.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://icl.ydjk.org.cn

TS:   /error/gim
来源：http://jce.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lde.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vvq.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://azp.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nos.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://jjg.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mrl.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rwm.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ipj.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nug.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://amu.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cvu.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zwh.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aky.xziqi.cn

================================================================================
来源：http://zzh.zdbjq.cn

J. 日期与时间
来源：http://tqq.iojbl.cn

================================================================================
来源：http://dur.gotoacloud.top

[J01] 获取当前时间
来源：http://yfq.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pso.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yfh.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://tch.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://mid.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jfu.andypj.xyz

Go:   time.Now()
来源：http://ljp.zhijiandao.cn

Ruby: Time.now
来源：http://ops.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vmf.bjfxy.top

[J02] 格式化输出
来源：http://knh.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://efe.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ogy.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uaj.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://lcz.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uur.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gvc.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lnn.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wxz.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://ghr.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ups.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xjq.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://gzb.cashguo.top

TS:   new Date("2024-01-02")
来源：http://woo.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://mtn.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sos.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://bwy.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://koz.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://mfp.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tke.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://czy.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nun.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kke.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eba.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lec.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://awr.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jff.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://szp.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://bnu.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cfm.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dak.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eop.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://rsa.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sto.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://kzq.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uts.yanxiufei.cn

[J06] 计算两时间之差
来源：http://apd.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://rxf.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://prs.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bos.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bfl.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://vha.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://efc.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://kes.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://sjv.tanke756.top

[J07] 比较两个日期
来源：http://zpi.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://nil.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bcc.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yqz.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ebb.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://anl.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://doq.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://urg.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://nio.zhengqikj.top

[J08] 提取年月日与星期
来源：http://xxi.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fsl.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rsa.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fnc.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qnv.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hpr.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mht.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vgh.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://klk.yuanzhike.top

[J09] 时区处理
来源：http://siz.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pmc.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qkn.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hvw.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tmm.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ynz.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gks.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uhh.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cdw.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://qwu.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bog.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lzx.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jop.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nks.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://muq.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rff.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ozn.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yuh.xuetiantiany.cn

================================================================================
来源：http://mtj.xuetiantiany.cn

K. JSON 与序列化
来源：http://joo.shangyingyoupin.top

================================================================================
来源：http://gpy.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://vtk.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dhf.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zfv.pycfn.com

JS:   JSON.stringify(obj)
来源：http://hax.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://tau.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ssc.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://dzz.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://ezq.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://npm.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://gbz.xylfe.cn

Py:   json.loads(s)
来源：http://wmr.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iby.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://hfo.zhiwuduotai.top


<!-- 参考信息 -->