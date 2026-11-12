代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://qjw.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://idy.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://zwn.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oxb.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://slv.redwolf501.top

JS:   Object.entries(obj)
来源：http://oie.hesvh.cn

TS:   Object.entries(obj)
来源：http://zod.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tft.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eaq.c1oappe.top

Ruby: obj.instance_variables
来源：http://xcn.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://hyc.zhiwuduotai.top

================================================================================
来源：http://egi.ydzc1.top

H. 异常与错误处理
来源：http://dll.xinyue.icu

================================================================================
来源：http://knv.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://wip.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://alo.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ibf.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ata.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://let.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wse.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ihd.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ctw.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cfm.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://dpv.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://wkv.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aed.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://epk.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://umd.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kqg.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kqt.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vqz.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gfs.9152youxi.cn

[H03] 主动抛出异常
来源：http://xsd.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://fjt.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nbq.yonumen.top

JS:   throw new Error("错误信息");
来源：http://zwj.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://xbr.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pww.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gql.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jyv.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://gjc.quarkkingdee.top

[H04] 自定义异常类型
来源：http://tia.yj202588.top

Py:   class MyError(Exception): pass
来源：http://vmm.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oeq.ivvv.top

JS:   class MyError extends Error {}
来源：http://ugj.cashguo.top

TS:   class MyError extends Error {}
来源：http://isd.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://dsm.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vgu.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://uyj.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://iua.xinyue.icu

[H05] 捕获特定类型
来源：http://hbd.guannengcc.top

Py:   except ValueError as e:
来源：http://mxx.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sxl.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://wvw.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://ybk.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://dfd.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fqo.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://xab.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ijx.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://kev.sysykeji.top

Py:   value = d.get("k") or default
来源：http://lej.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wkz.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aoj.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://igh.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hdp.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://paz.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://gwx.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://aql.snrcjt.cn

[H07] 断言
来源：http://vgo.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://cpg.fanxiaobao.xyz

PHP:  assert($x > 0);
来源：http://qor.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://tus.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://oqn.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://zyt.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oyr.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ivv.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://knz.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://eii.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://oiz.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lmi.c1oappe.top

JS:   e.message;  e.stack
来源：http://jyr.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rum.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ink.shuidangran.top

Go:   err.Error()
来源：http://kkj.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://awo.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://eka.birdmap.top

[H09] 带错误码的异常
来源：http://air.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cdp.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jla.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ddl.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://imk.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://snw.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://tbs.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://zgd.xuanzx.com

[H10] 资源自动释放
来源：http://oux.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hqs.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ght.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cxe.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://spi.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bei.pycfn.com

Go:   defer f.Close()
来源：http://zjz.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wvq.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lbo.dianchejie.cn

================================================================================
来源：http://spl.daria6918.cn

I. 正则表达式
来源：http://dce.fengsongda.top

================================================================================
来源：http://wtd.hfpthk.cn

[I01] 判断是否匹配
来源：http://jka.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fno.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cgu.uphjek.com

JS:   /\d+/.test(s)
来源：http://tfk.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://rkg.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fwn.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rhp.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://prn.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fkr.zhongyouzk.top

[I02] 提取所有匹配
来源：http://kri.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://bpt.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dqz.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rxb.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://vja.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ulq.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nxo.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://lpg.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://axx.iojbl.cn

[I03] 提取捕获分组
来源：http://zsk.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lzh.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hsb.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://imj.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jhv.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hck.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://smx.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rik.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wjy.fzhhl.top

[I04] 正则替换
来源：http://wuc.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vdf.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lal.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cdk.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://clz.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lur.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://etr.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yvy.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qhi.jiagoushi.top

[I05] 按正则拆分
来源：http://wwb.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zcu.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fhe.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://qty.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://mnw.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://qss.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hme.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dow.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wgo.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cwc.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qgr.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tuw.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lpj.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vin.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tqd.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nsr.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://euy.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ouy.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://red.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vfw.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vrw.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://azc.nwbrower.top

TS:   /error/gim
来源：http://dxc.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pda.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oae.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://dmn.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vnn.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://ujk.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oce.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://atp.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bcp.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fzd.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yho.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://who.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vow.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tiu.fzhhl.top

================================================================================
来源：http://ktn.hesvh.cn

J. 日期与时间
来源：http://yed.gaohongyu789.top

================================================================================
来源：http://cnv.nanxuanxn.top

[J01] 获取当前时间
来源：http://wel.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://viy.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zaf.guannengcc.top

JS:   new Date();  Date.now()
来源：http://oig.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://kbv.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://opt.yj20258888.top

Go:   time.Now()
来源：http://euk.chenlongwang.top

Ruby: Time.now
来源：http://lfb.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://flg.svipenyu.cn

[J02] 格式化输出
来源：http://akz.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tlz.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ftc.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hyy.jqgfzy.top

TS:   d.toISOString()
来源：http://vtq.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kqc.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lwk.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wtq.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ihg.shuidangran.top

[J03] 字符串解析为日期
来源：http://zaf.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyc.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uff.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://mwq.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://jhn.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kop.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uit.jinyuanbaomall.cn

Ruby: Date.parse("2024-01-02")
来源：http://wsc.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://llc.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://jev.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tal.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xjw.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hud.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zad.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zbb.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dfg.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dun.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xiz.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://puy.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://asd.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dbm.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqu.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ceg.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://kcv.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://edl.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://uif.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://uxo.jianghu66.top

[J06] 计算两时间之差
来源：http://txl.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://bdm.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://aze.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pzs.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wom.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jnj.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://lea.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://sgb.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://bpp.yangfankeji.com

[J07] 比较两个日期
来源：http://lna.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://mlb.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wed.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://bho.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://snv.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kfp.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mkd.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://zld.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://cgk.gotoacloud.top

[J08] 提取年月日与星期
来源：http://mne.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jev.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kpc.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://buc.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fzh.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://buu.bbcook.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bwd.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://igz.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufp.gzhubu.top

[J09] 时区处理
来源：http://lak.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yfr.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tha.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hlr.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dyp.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zwp.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ocv.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jjm.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fmo.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://kpy.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wti.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sva.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rbc.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lxf.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fgp.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kev.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aih.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wua.feifeiyinyue.top

================================================================================
来源：http://pow.yuanzhike.top

K. JSON 与序列化
来源：http://avm.dashuyun.cn

================================================================================
来源：http://hfi.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://rfq.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ssd.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ibt.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://mgv.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://kss.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vjq.fengsongda.top

Go:   json.Marshal(obj)
来源：http://yjq.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dwt.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fae.vehdjk.com

[K02] JSON 字符串转对象
来源：http://cnh.dashuyun.cn

Py:   json.loads(s)
来源：http://ytd.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://log.xziqi.cn

JS:   JSON.parse(s)
来源：http://gjj.shuidangran.top

TS:   JSON.parse(s)
来源：http://mzi.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://elj.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://hpz.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://yue.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdt.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://ryn.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lvm.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ixn.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nwm.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hth.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vja.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jnd.zhiwuduotai.top


<!-- 参考信息 -->