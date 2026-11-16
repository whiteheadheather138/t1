代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://ljk.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://loi.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://jjq.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://alb.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://iom.yj20258888.top

JS:   Object.entries(obj)
来源：http://vst.jinyuanbaomall.cn

TS:   Object.entries(obj)
来源：http://awm.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bby.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zmw.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://dkw.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://tzv.c1oappe.top

================================================================================
来源：http://rdb.ctjpmb.com

H. 异常与错误处理
来源：http://mgy.cashguo.top

================================================================================
来源：http://pmp.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://lqx.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hlh.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tqq.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jel.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eje.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iob.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bly.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://agw.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxi.fehbvm.com

[H02] finally / ensure 收尾
来源：http://pwo.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tsa.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jkr.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wpo.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cng.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aue.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hoq.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dzy.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://iaw.zhoulong.xyz

[H03] 主动抛出异常
来源：http://hki.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://dba.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uiz.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://vrl.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://ypa.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uyl.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mip.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zio.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://ndv.hysaishi.cn

[H04] 自定义异常类型
来源：http://ull.sweek.top

Py:   class MyError(Exception): pass
来源：http://uqk.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://riy.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://ugw.fengsongda.top

TS:   class MyError extends Error {}
来源：http://lqr.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://poi.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lrp.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://nxf.aizwys.cn

C#:   class MyException : Exception {}
来源：http://lyu.shzxlz.cn

[H05] 捕获特定类型
来源：http://elj.quarkkingdee.top

Py:   except ValueError as e:
来源：http://nev.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ogz.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://fmv.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://udv.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://xte.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iqi.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://cyn.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://efi.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://beb.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://emj.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://zxg.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://eya.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wxf.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cor.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zuj.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://gfj.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://dnq.jianghu66.top

[H07] 断言
来源：http://mju.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://nsg.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://zia.jinyuanbaomall.cn

JS:   console.assert(x > 0);
来源：http://avo.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://bry.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://fji.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yml.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iwy.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://rme.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://ljj.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://usi.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sro.fehbvm.com

JS:   e.message;  e.stack
来源：http://ymr.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kyk.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://hwn.hesvh.cn

Go:   err.Error()
来源：http://kyu.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://ufx.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://spz.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://yde.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zxq.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uwe.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ydb.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iav.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://red.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vwg.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://fdm.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://drq.ydzc1.top

[H10] 资源自动释放
来源：http://zka.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://oxj.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gmi.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nol.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rvq.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gjn.dashuyun.cn

Go:   defer f.Close()
来源：http://sle.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ywa.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rgn.aizwys.cn

================================================================================
来源：http://wud.yueranfly.top

I. 正则表达式
来源：http://jcg.yanxiufei.cn

================================================================================
来源：http://hve.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://qrm.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://brz.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://khn.meibo888.top

JS:   /\d+/.test(s)
来源：http://dtf.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://oue.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jns.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nym.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://fcx.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xvw.yvedp.cn

[I02] 提取所有匹配
来源：http://bcw.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://aiu.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xjw.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://agj.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://dij.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dnv.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sqw.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://zdk.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fnd.fengsongda.top

[I03] 提取捕获分组
来源：http://meo.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xqb.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kmd.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dto.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hft.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://chs.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://flv.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://juc.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://prh.yonumen.top

[I04] 正则替换
来源：http://ryg.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vqy.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xjn.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://ckg.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://lcg.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rgg.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gmy.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://euu.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jvd.zhiwuduotai.top

[I05] 按正则拆分
来源：http://qyc.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gxd.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tvs.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://omx.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://rwh.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://qom.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zfy.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zpt.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mdx.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jrg.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zqj.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fnn.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wfv.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rdw.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zwu.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mtp.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xxr.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cne.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://kme.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eit.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tiy.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dqh.quarkkingdee.top

TS:   /error/gim
来源：http://kat.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://onp.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://upj.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://iws.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ozh.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://zrj.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rmf.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sez.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zfb.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xvx.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uza.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bgi.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sib.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jhy.quarkkingdee.top

================================================================================
来源：http://oeq.zhaomingkeji.xyz

J. 日期与时间
来源：http://tbc.chenzaomai.com

================================================================================
来源：http://qgw.uphjek.com

[J01] 获取当前时间
来源：http://zvu.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://krz.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ylb.jianghu66.top

JS:   new Date();  Date.now()
来源：http://gyr.smart0.xyz

TS:   new Date();  Date.now()
来源：http://qek.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zfc.jinqigfzy.top

Go:   time.Now()
来源：http://cjf.fktsv.cn

Ruby: Time.now
来源：http://jex.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kox.zhiwuduotai.top

[J02] 格式化输出
来源：http://pdp.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sav.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xct.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qln.hcnkem.com

TS:   d.toISOString()
来源：http://vsu.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kvg.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://roy.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zxb.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fpg.bbcook.cn

[J03] 字符串解析为日期
来源：http://hek.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mpj.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qvw.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://taf.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://ybi.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://vcy.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vle.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://lte.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wkl.guannengcc.top

[J04] 时间戳与日期互转
来源：http://grh.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://soi.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jhh.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aom.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qjr.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://snz.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tdp.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dbu.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgm.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://ymf.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://sfa.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://byz.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ryx.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gie.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://sxq.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ggc.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://bxu.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://boz.dianchejie.cn

[J06] 计算两时间之差
来源：http://zzo.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://erh.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://bek.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dsu.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://khu.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://tnn.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://eao.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://oom.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://epl.hammf.cn

[J07] 比较两个日期
来源：http://dnz.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://lyp.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fju.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iyi.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://omz.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qhz.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mjv.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://kpv.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ucs.hywenlv.cn

[J08] 提取年月日与星期
来源：http://vax.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://svr.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mag.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ttp.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kkv.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qqd.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pxi.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sob.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nqo.svipenyu.cn

[J09] 时区处理
来源：http://ofw.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gpn.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hvu.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xch.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpy.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hpi.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lko.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://kxk.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zuz.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://kqn.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ypb.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jvf.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://avi.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aou.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dev.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mql.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zsh.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xsn.feifeiyinyue.top

================================================================================
来源：http://eoj.dashuyun.cn

K. JSON 与序列化
来源：http://mzw.sufxvd.cn

================================================================================
来源：http://chs.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://moy.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sgh.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cfk.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://ivs.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://uzi.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xdw.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://nuh.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qzg.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vgw.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://qlf.hammf.cn

Py:   json.loads(s)
来源：http://yrl.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxp.bjfxy.top

JS:   JSON.parse(s)
来源：http://cga.svipenyu.cn

TS:   JSON.parse(s)
来源：http://sub.xinyue.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gzm.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://cve.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://eoa.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hqe.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://hoc.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yik.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nor.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dqf.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ral.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aom.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mfh.chenzaomai.com


<!-- 参考信息 -->