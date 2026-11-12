代发 wailian999

PHP:  get_object_vars($obj);
来源：http://eza.yj202588.top

JS:   Object.entries(obj)
来源：http://jim.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://rhh.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ims.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://piu.yueranfly.top

Ruby: obj.instance_variables
来源：http://tiu.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://tiu.wangshuangyany.cn

================================================================================
来源：http://jkb.aibaodan.cn

H. 异常与错误处理
来源：http://anu.zdbjq.cn

================================================================================
来源：http://dqs.hammf.cn

[H01] try / catch 基础
来源：http://jjf.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zfp.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgg.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ksb.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hgm.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tux.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qpa.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mbd.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://amg.uphjek.com

[H02] finally / ensure 收尾
来源：http://rxn.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://fdl.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bce.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kvd.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://txh.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qyt.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yew.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://qmo.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cgp.meibo888.top

[H03] 主动抛出异常
来源：http://ycf.cdnleiting.top

Py:   raise ValueError("错误信息")
来源：http://mbt.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://esq.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://uqg.yj20258.top

TS:   throw new Error("错误信息");
来源：http://hsp.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uwz.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dlg.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ryv.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hkg.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://xog.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://hcl.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://bpg.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://zyh.epnwcf.com

TS:   class MyError extends Error {}
来源：http://rci.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://vpd.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://glg.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://hzg.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://wlu.daxiang520.top

[H05] 捕获特定类型
来源：http://jso.haohaochexian.top

Py:   except ValueError as e:
来源：http://pfg.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ejk.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://lzj.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ali.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://rmj.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sxy.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://cul.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lia.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://rax.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://tcs.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ufb.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://huk.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aty.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vkt.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hzt.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://mxs.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://pff.ywan-chungtsiang.top

[H07] 断言
来源：http://bzd.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://miu.gotoacloud.top

PHP:  assert($x > 0);
来源：http://ucp.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://tnp.bjfxy.top

TS:   console.assert(x > 0);
来源：http://uqx.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://ehx.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rre.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xmg.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://xnb.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://edo.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://quu.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vsq.sweek.top

JS:   e.message;  e.stack
来源：http://jud.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vvn.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kzg.yuxming.cn

Go:   err.Error()
来源：http://yok.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://dpf.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://qwp.vehdjk.com

[H09] 带错误码的异常
来源：http://hch.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://civ.gogol.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ybk.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dqo.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oij.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://psn.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zpg.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eri.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wom.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://cbq.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://omc.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pfb.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vbe.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wio.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://skx.ivvv.top

Go:   defer f.Close()
来源：http://yqv.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dji.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bqq.xinyue.icu

================================================================================
来源：http://etf.jinyuanbaomall.cn

I. 正则表达式
来源：http://ysx.yvedp.cn

================================================================================
来源：http://ijo.chenzaomai.com

[I01] 判断是否匹配
来源：http://zvd.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ixc.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yif.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://cek.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://ffh.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zjg.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cnh.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://cxv.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hwb.shuidangran.top

[I02] 提取所有匹配
来源：http://reg.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://tvs.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xdx.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://msf.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://npy.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rjj.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nks.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://jsb.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xtp.zdbjq.cn

[I03] 提取捕获分组
来源：http://vdm.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fnj.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nhh.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zng.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eyi.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dcm.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fsf.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vkt.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ozw.birdmap.top

[I04] 正则替换
来源：http://xwi.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vdl.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nkl.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://nbs.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://acf.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eke.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gtp.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lxw.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uwi.sxryk.cn

[I05] 按正则拆分
来源：http://pub.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fhi.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yxt.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://yag.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://mju.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://czw.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://phs.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://ulf.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://itl.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qrj.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ffn.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hoh.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hiq.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vrb.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wxc.hammf.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qgk.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qmv.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eju.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://ehx.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rrr.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://krh.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dlp.daria6918.cn

TS:   /error/gim
来源：http://uwz.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ahw.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://psa.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://fgf.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zge.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://raz.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yxo.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://euw.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qac.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bym.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nrj.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jdt.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hsm.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rgz.cheryme.top

================================================================================
来源：http://pzn.sysykeji.top

J. 日期与时间
来源：http://ect.tarul.cn

================================================================================
来源：http://bla.jiagoushi.top

[J01] 获取当前时间
来源：http://nam.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sxd.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xxy.sxryk.cn

JS:   new Date();  Date.now()
来源：http://cik.vehdjk.com

TS:   new Date();  Date.now()
来源：http://sou.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ipb.hnqzz.top

Go:   time.Now()
来源：http://rne.nanxinkj.top

Ruby: Time.now
来源：http://ryx.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kyb.fengsongda.top

[J02] 格式化输出
来源：http://loc.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://agf.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lez.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tnt.jqgfzy.top

TS:   d.toISOString()
来源：http://fka.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fah.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gwy.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jzx.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wfe.yj20258.top

[J03] 字符串解析为日期
来源：http://pel.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pod.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pdu.sweek.top

JS:   new Date("2024-01-02")
来源：http://atw.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://obj.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://mgw.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://miv.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://tgs.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jeq.redwolf501.top

[J04] 时间戳与日期互转
来源：http://bcc.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nhm.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://irt.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://exz.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nil.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sex.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qep.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zqt.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dke.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://hjk.ivvv.top

Py:   now + timedelta(days=7)
来源：http://ofy.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yuf.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujq.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ghx.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://edy.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xri.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://iyn.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://pib.yfazqb.com

[J06] 计算两时间之差
来源：http://bag.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://haw.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://jcc.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wkf.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tpb.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://bwm.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://rql.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://skr.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://afx.zdbjq.cn

[J07] 比较两个日期
来源：http://vij.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://sbe.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vas.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wtu.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://gvk.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tbi.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdi.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://cqe.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://jze.guowangkeji.top

[J08] 提取年月日与星期
来源：http://vpr.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bsr.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://onc.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pec.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oil.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ydf.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zni.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rlg.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wfc.iojbl.cn

[J09] 时区处理
来源：http://chx.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bsw.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qxw.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmc.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmw.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dfw.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lcs.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vyu.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hrc.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://qcg.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nze.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lym.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uzu.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cof.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pxp.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://anv.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bua.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kpo.tanke756.top

================================================================================
来源：http://txk.ybcxt.top

K. JSON 与序列化
来源：http://kxh.hfpthk.cn

================================================================================
来源：http://xyp.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://uil.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ere.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://non.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://nhs.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://elm.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lyk.fengsongda.top

Go:   json.Marshal(obj)
来源：http://jbo.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://war.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ale.meibo888.top

[K02] JSON 字符串转对象
来源：http://uai.pengpengdd.cyou

Py:   json.loads(s)
来源：http://ydu.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xar.svipenyu.cn

JS:   JSON.parse(s)
来源：http://pdx.cqqwz.cn

TS:   JSON.parse(s)
来源：http://yaf.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vmx.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://kgw.shuidangran.top

Ruby: JSON.parse(s)
来源：http://pdl.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jrq.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://kpq.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xrx.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jzw.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lsa.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iet.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lxr.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ued.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hse.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mue.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://hjs.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qws.yj20258888.top


<!-- 参考信息 -->