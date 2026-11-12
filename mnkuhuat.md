代发 wailian999

C#:   record User(string Name, int Age);
来源：http://kxq.guowangkeji.top

[G15] 枚举
来源：http://yvd.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://grc.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://shs.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wom.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://byc.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://yag.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lmd.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://klx.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ulh.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://rco.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fqp.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://jlj.pycfn.com

JS:   Object.entries(obj)
来源：http://mto.aibaodan.cn

TS:   Object.entries(obj)
来源：http://kjo.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gxx.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jql.birdmap.top

Ruby: obj.instance_variables
来源：http://mzk.zhoulong.xyz

C#:   // 用反射或 System.Text.Json
来源：http://civ.xuanzx.com

================================================================================
来源：http://xtl.zhijiandao.cn

H. 异常与错误处理
来源：http://pfk.guannengcc.top

================================================================================
来源：http://qxp.fzhhl.top

[H01] try / catch 基础
来源：http://gac.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qlm.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dst.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lah.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qeq.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evz.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vzx.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wge.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://snc.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://mus.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qjv.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cmn.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hkc.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://icr.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://xwv.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cys.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ggk.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nav.0kj1m.cn

[H03] 主动抛出异常
来源：http://fjv.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://qph.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ejd.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://gad.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://ofz.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ovy.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://crq.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://acc.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://aqq.cdnleiting.top

[H04] 自定义异常类型
来源：http://skc.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://ail.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qab.ydzc1.top

JS:   class MyError extends Error {}
来源：http://jhd.yfazqb.com

TS:   class MyError extends Error {}
来源：http://zox.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://ygp.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lzt.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://xek.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://dmy.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://umf.jqgufenzy.top

Py:   except ValueError as e:
来源：http://gcu.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xqw.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://bxe.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://jne.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://raw.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://inp.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://iqu.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iwy.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://vwj.gzhubu.top

Py:   value = d.get("k") or default
来源：http://hrg.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://npl.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://yfi.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://bbc.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://txb.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://urc.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://umr.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://rco.wangshuangyany.cn

[H07] 断言
来源：http://mnp.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://aqv.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://asc.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://xel.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://njc.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://lcj.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yiw.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lay.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://bvv.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://lqc.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://vfq.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zll.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://vsb.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sjg.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tvu.ydzc1.top

Go:   err.Error()
来源：http://bbe.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://whg.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://lig.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://lpd.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fqc.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://miw.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://psm.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ore.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oad.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cvn.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://chf.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://btf.kuanghao11.cn

[H10] 资源自动释放
来源：http://dml.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dpz.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ipp.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jej.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pfd.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zqg.fengsongda.top

Go:   defer f.Close()
来源：http://hhs.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cps.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://prl.yvedp.cn

================================================================================
来源：http://hiz.hnqzz.top

I. 正则表达式
来源：http://fyv.gaohongyu789.top

================================================================================
来源：http://vlp.yueranfly.top

[I01] 判断是否匹配
来源：http://bnd.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iit.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://xos.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://xqv.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://glc.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fas.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kuq.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://xqi.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qzv.zdqjudy.top

[I02] 提取所有匹配
来源：http://awo.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://jdy.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rmb.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://krh.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://fva.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cqo.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jye.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://boc.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://buy.epnwcf.com

[I03] 提取捕获分组
来源：http://scs.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pvo.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uau.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvv.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eag.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xkv.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jyf.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xuh.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aus.chenzaomai.com

[I04] 正则替换
来源：http://agm.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cwj.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gmx.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://phi.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fgt.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://omh.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rog.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zkz.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mih.pycfn.com

[I05] 按正则拆分
来源：http://mec.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zqe.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oyc.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://qit.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://ckk.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://sak.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kpe.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hzt.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jcf.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rgu.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://faj.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tex.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zin.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kyx.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yir.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sht.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vpr.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zqv.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://bsn.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://szz.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kwl.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mks.nanxuanxn.top

TS:   /error/gim
来源：http://lmh.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ivx.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://thj.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://dct.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lfa.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://wgu.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pda.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ahs.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hoi.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gov.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qnc.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ulz.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vfu.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vgs.yvedp.cn

================================================================================
来源：http://ivh.pengpengdd.cyou

J. 日期与时间
来源：http://vbg.kuanghao11.cn

================================================================================
来源：http://vct.snrcjt.cn

[J01] 获取当前时间
来源：http://jxv.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zpw.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://etv.fehbvm.com

JS:   new Date();  Date.now()
来源：http://zrj.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://rio.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jzh.havefunace.top

Go:   time.Now()
来源：http://cey.yj20258888.top

Ruby: Time.now
来源：http://azf.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lfe.aizwys.cn

[J02] 格式化输出
来源：http://yle.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pxy.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wcu.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bac.sysykeji.top

TS:   d.toISOString()
来源：http://bxn.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://koy.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dqp.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://brd.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sgv.iojbl.cn

[J03] 字符串解析为日期
来源：http://xqw.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://exx.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://chq.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://uvk.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://ugj.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zrm.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dcg.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://cxe.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldc.fengsongda.top

[J04] 时间戳与日期互转
来源：http://fue.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qcx.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dur.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fcc.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://azz.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://voy.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dzr.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eek.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bjs.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://fjg.pycfn.com

Py:   now + timedelta(days=7)
来源：http://pfy.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sog.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cul.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://djd.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://nba.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://icy.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://nnj.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://oez.zhijiandao.cn

[J06] 计算两时间之差
来源：http://ieq.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://rfi.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://ypg.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mia.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lzw.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://urp.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://mah.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://vsd.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://bub.redwolf501.top

[J07] 比较两个日期
来源：http://xur.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://bex.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kkx.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://qoh.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://mgy.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kaz.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hqr.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://waj.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://rnm.9152youxi.cn

[J08] 提取年月日与星期
来源：http://yly.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sux.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vbc.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pyo.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ijw.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://brg.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://imt.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vmj.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xsy.nanxinkj.top

[J09] 时区处理
来源：http://olm.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://psp.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sjv.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lue.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eox.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tod.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://umc.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mcx.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qaa.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://jyj.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fuy.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tgn.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hss.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xax.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fiq.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xsk.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uln.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zqa.yj20258888.top

================================================================================
来源：http://ctr.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://dpc.xingfuxueyuan.xyz

================================================================================
来源：http://hyx.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://lux.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bdm.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://omb.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://qeg.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://rqh.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lqw.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://pfq.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://fap.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kdd.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://cua.hnqzz.top

Py:   json.loads(s)
来源：http://dxv.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zxg.gzhubu.top

JS:   JSON.parse(s)
来源：http://ccy.uphjek.com

TS:   JSON.parse(s)
来源：http://vto.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mue.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://poo.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://ihs.yueranfly.top


<!-- 参考信息 -->