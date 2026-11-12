代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://shd.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://azs.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://llx.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qkm.cheryme.top

PHP:  get_object_vars($obj);
来源：http://fnj.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://ahn.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://pdh.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jgs.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://nwe.yuanzhike.top

Ruby: obj.instance_variables
来源：http://yuy.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://rng.uphjek.com

================================================================================
来源：http://dtb.daxiang520.top

H. 异常与错误处理
来源：http://nfl.fktsv.cn

================================================================================
来源：http://ucm.fktsv.cn

[H01] try / catch 基础
来源：http://lhk.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pvk.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lbb.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cqj.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lip.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nek.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://trv.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qst.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pmo.yueranfly.top

[H02] finally / ensure 收尾
来源：http://vmt.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://dyk.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://wdd.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ozc.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tbl.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://yvc.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://cbp.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vxo.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gnx.pycfn.com

[H03] 主动抛出异常
来源：http://eip.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://duq.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zvm.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://nvh.meibo888.top

TS:   throw new Error("错误信息");
来源：http://bje.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://myz.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pvh.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kbk.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kpg.gotoacloud.top

[H04] 自定义异常类型
来源：http://wwd.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://vba.sufxvd.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mtq.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://exp.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://vjm.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://ohw.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mdj.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://ecr.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://fru.hammf.cn

[H05] 捕获特定类型
来源：http://qov.wangdashe.top

Py:   except ValueError as e:
来源：http://cmb.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mth.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://qgy.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://nra.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://bnd.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dkj.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://chz.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ajz.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://xzz.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://nhi.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wnc.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://hxz.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://aof.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lac.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qen.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://xio.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://cpw.dianchejie.cn

[H07] 断言
来源：http://hwy.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://dos.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://jku.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://vaf.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://bdy.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://pro.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tst.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://kba.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://ltc.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://ppl.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://hyq.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oqe.cashguo.top

JS:   e.message;  e.stack
来源：http://ylj.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uda.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xxg.pengpengdd.cyou

Go:   err.Error()
来源：http://yvb.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://gsz.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://ati.yvedp.cn

[H09] 带错误码的异常
来源：http://gan.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tvv.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eok.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ewx.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ffi.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gsz.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pgg.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://qxl.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rtu.yangfankeji.com

[H10] 资源自动释放
来源：http://upv.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://upa.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tfm.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xtn.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uyz.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xim.ehwqpu.com

Go:   defer f.Close()
来源：http://srt.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bei.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wec.jqgfzy.top

================================================================================
来源：http://rqu.sysykeji.top

I. 正则表达式
来源：http://orv.xziqi.cn

================================================================================
来源：http://ihc.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://fsr.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ukx.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://car.aizwys.cn

JS:   /\d+/.test(s)
来源：http://zlu.xylfe.cn

TS:   /\d+/.test(s)
来源：http://vrl.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bdb.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ejd.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://gvc.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wuf.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://ckg.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://hjb.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nkt.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyp.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://utu.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tfr.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://noz.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://utm.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lih.quarkkingdee.top

[I03] 提取捕获分组
来源：http://vlz.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vbm.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://npv.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jqo.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hcn.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ekq.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bpq.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vby.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dbh.redwolf501.top

[I04] 正则替换
来源：http://tpb.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mtg.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wkb.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kzb.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dje.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://pff.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ltd.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mjs.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xmx.hfpthk.cn

[I05] 按正则拆分
来源：http://afe.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wnj.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mct.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://llm.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://xic.shanyushiyangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://ouj.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nxh.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://prw.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hor.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mei.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://enp.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://prd.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xjy.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yst.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mor.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wqk.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kgd.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qmi.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://dfk.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://khp.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://otx.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://awi.wangshuangyany.cn

TS:   /error/gim
来源：http://bwd.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aqm.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ekf.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://idp.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://acx.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://tfx.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imi.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lly.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://utl.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://crp.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dgs.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iep.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kve.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jrj.vqdsnc.cn

================================================================================
来源：http://fld.ywan-chungtsiang.top

J. 日期与时间
来源：http://dcw.gotoacloud.top

================================================================================
来源：http://sqb.yvedp.cn

[J01] 获取当前时间
来源：http://ptu.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://znu.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jwi.epnwcf.com

JS:   new Date();  Date.now()
来源：http://izk.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://ieh.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kgv.yj202588.top

Go:   time.Now()
来源：http://uqv.fehbvm.com

Ruby: Time.now
来源：http://wmg.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ojg.jqgfzy.top

[J02] 格式化输出
来源：http://kdf.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fih.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ltg.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bcg.ydzc1.top

TS:   d.toISOString()
来源：http://pzz.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jhp.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xvp.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mbv.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://csp.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://ozm.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zmr.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ihp.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://bvy.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://ryg.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://kov.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdg.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://hwt.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://auz.yj202588.top

[J04] 时间戳与日期互转
来源：http://mcd.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sjn.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ofl.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bgr.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jev.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lmq.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://klc.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ypa.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kjq.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://tti.cheryme.top

Py:   now + timedelta(days=7)
来源：http://anx.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hfb.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ijg.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fzp.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://zvo.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rzq.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://aon.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://gui.yj202588.top

[J06] 计算两时间之差
来源：http://ogt.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://zoq.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://tvm.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://msy.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zzs.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://zkq.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://jav.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://utr.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://vwk.yuanzhike.top

[J07] 比较两个日期
来源：http://gus.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://wnl.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://imn.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zaf.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://iyy.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yrs.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pth.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://ryc.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://vtr.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://ltl.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nng.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://usx.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fxp.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pfq.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aol.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wkl.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jrk.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jcc.yangfankeji.com

[J09] 时区处理
来源：http://plr.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ezh.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kww.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iip.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hcc.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://smq.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aia.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yuj.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uzo.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://too.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ilm.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ksr.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nih.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fcz.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgq.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nwx.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hpr.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ugd.zhoulong.xyz

================================================================================
来源：http://ctc.wangdashe.top

K. JSON 与序列化
来源：http://kyf.ywan-chungtsiang.top

================================================================================
来源：http://npn.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://zkl.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cny.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jfx.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://pvl.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://lrn.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gur.birdmap.top

Go:   json.Marshal(obj)
来源：http://wit.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://lnu.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gpa.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://bnb.xziqi.cn

Py:   json.loads(s)
来源：http://thm.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zdy.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://hel.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://dco.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aru.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://rga.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://pud.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sgo.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://dct.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://clt.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ibe.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cvz.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vop.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xjh.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lfd.snrcjt.cn


<!-- 参考信息 -->