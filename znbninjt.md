代发 wailian999

[G14] 数据类 / record
来源：http://acp.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://svs.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://obw.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://aoi.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://bfn.52xcode.cn

Java: record User(String name, int age) {}
来源：http://yut.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://ivp.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gdc.jinghuilouyu.cn

C#:   record User(string Name, int Age);
来源：http://btz.epnwcf.com

[G15] 枚举
来源：http://zvm.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tap.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mlu.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cjg.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hah.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://sbq.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hxp.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://lwx.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://svp.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://cgp.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rhi.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://cfv.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://hst.haohaochexian.top

TS:   Object.entries(obj)
来源：http://epf.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uib.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ydp.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://oaz.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://ajt.yuanzhike.top

================================================================================
来源：http://dok.nanxuanxn.top

H. 异常与错误处理
来源：http://mpa.sufxvd.cn

================================================================================
来源：http://qpo.vqdsnc.cn

[H01] try / catch 基础
来源：http://drn.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eiz.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tsx.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ktt.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nac.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yco.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://opk.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mpx.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sfp.mhx1999.top

[H02] finally / ensure 收尾
来源：http://vdv.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ngl.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jth.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kyh.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://mbi.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ghm.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://unw.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://riy.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://htl.wangdashe.top

[H03] 主动抛出异常
来源：http://anq.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://lfc.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ogo.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://iex.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://khm.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pas.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fcs.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://luc.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vsf.tanke756.top

[H04] 自定义异常类型
来源：http://hvs.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://bhx.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://irs.sxryk.cn

JS:   class MyError extends Error {}
来源：http://ler.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://eua.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://zwv.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wdb.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://zjt.cheryme.top

C#:   class MyException : Exception {}
来源：http://kfo.vehdjk.com

[H05] 捕获特定类型
来源：http://znl.gotoacloud.top

Py:   except ValueError as e:
来源：http://cbm.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vru.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://xug.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://sbz.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://whm.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bnu.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://ixl.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ypq.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://xsi.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://hya.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://xxd.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://nck.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://qcx.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lwt.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ohl.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://vps.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://qby.shuidangran.top

[H07] 断言
来源：http://qjg.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://nkf.shuidangran.top

PHP:  assert($x > 0);
来源：http://ojb.tarul.cn

JS:   console.assert(x > 0);
来源：http://xmn.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://cck.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://zwf.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vku.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://wcq.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://aex.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://xpi.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://aeg.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fev.hammf.cn

JS:   e.message;  e.stack
来源：http://tia.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://pbn.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sqx.gotoacloud.top

Go:   err.Error()
来源：http://mjp.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://slc.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://xqw.nanxinkj.top

[H09] 带错误码的异常
来源：http://veh.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ctp.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://crk.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yvf.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://joz.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fci.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wjf.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kpi.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uaz.yvedp.cn

[H10] 资源自动释放
来源：http://bvo.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pzo.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iju.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://siv.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rrh.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kic.jyoumei.cn

Go:   defer f.Close()
来源：http://iob.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mso.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://udo.jinqigufen.top

================================================================================
来源：http://bdu.hcnkem.com

I. 正则表达式
来源：http://dcl.xziqi.cn

================================================================================
来源：http://cea.fzhhl.top

[I01] 判断是否匹配
来源：http://zku.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ndy.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://hfg.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://nuw.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://hsg.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://njj.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yeh.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://nvp.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bxc.redwolf501.top

[I02] 提取所有匹配
来源：http://qjw.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://bza.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wgn.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lnu.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://uxm.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eru.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bym.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://mbf.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pfo.ydjk.org.cn

[I03] 提取捕获分组
来源：http://fpd.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fno.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fhp.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dru.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fnl.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sfj.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tfy.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jgy.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bws.zycfv.cn

[I04] 正则替换
来源：http://fnp.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://smf.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pan.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://heg.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://dak.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sdk.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vjr.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://rfz.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cec.bjfxy.top

[I05] 按正则拆分
来源：http://eoc.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nmi.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ygt.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://eaz.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://zhq.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://orh.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hht.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://cpq.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lno.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eru.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://skm.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxc.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rqt.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bbx.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gcy.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://azk.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hdz.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aqc.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://fen.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mia.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fyn.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xgf.haohaochexian.top

TS:   /error/gim
来源：http://rnf.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tin.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fmf.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://ood.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://itg.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://mbh.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://boz.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mmg.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vwj.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vjd.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mnt.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ovg.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pyq.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dpt.feifeiyinyue.top

================================================================================
来源：http://mma.yj20258.top

J. 日期与时间
来源：http://gah.tarul.cn

================================================================================
来源：http://dvw.xziqi.cn

[J01] 获取当前时间
来源：http://jlp.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iyj.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gey.tarul.cn

JS:   new Date();  Date.now()
来源：http://dmo.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://yzi.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://snf.nanxuanxn.top

Go:   time.Now()
来源：http://hon.yfazqb.com

Ruby: Time.now
来源：http://bfd.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tnp.hywenlv.cn

[J02] 格式化输出
来源：http://dgp.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ggm.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://poo.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pty.snrcjt.cn

TS:   d.toISOString()
来源：http://zhl.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dfo.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hpt.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mob.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nvz.ydzc1.top

[J03] 字符串解析为日期
来源：http://qhn.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jvt.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tkx.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://bqn.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://cqc.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yrb.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rwp.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ngp.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qob.bjfxy.top

[J04] 时间戳与日期互转
来源：http://rar.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uzv.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://day.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rhl.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lkw.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uql.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ots.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pzi.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cfi.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://sui.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://dhq.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://lui.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hqe.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fuw.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://ofc.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tsl.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://gld.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://dxm.kuanghao11.cn

[J06] 计算两时间之差
来源：http://pto.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://zan.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://ffj.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jfo.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jik.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nvq.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://ian.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://efm.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://dca.cheryme.top

[J07] 比较两个日期
来源：http://fem.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://tnq.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hnf.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://yfe.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://rjh.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vdi.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tkj.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://qmg.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://mmz.hywenlv.cn

[J08] 提取年月日与星期
来源：http://bvw.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wwf.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tyg.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://miy.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cds.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aeb.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aph.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fhg.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xfj.cheryme.top

[J09] 时区处理
来源：http://uqy.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://msz.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wwh.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aed.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sqs.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fpu.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zrq.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ljm.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://apr.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://mvy.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oda.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://syw.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nia.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://adu.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xow.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://utm.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fdu.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nrm.fktsv.cn

================================================================================
来源：http://kxi.gogol.net.cn

K. JSON 与序列化
来源：http://iva.epnwcf.com

================================================================================
来源：http://dhy.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://ulc.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ela.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ciw.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://djy.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://smm.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ugn.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://wkn.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://piu.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uoj.hysaishi.cn


<!-- 参考信息 -->