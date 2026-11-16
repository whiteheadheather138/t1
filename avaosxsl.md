代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://spl.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://axv.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://eki.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vrp.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://dys.hcnkem.com

JS:   Object.entries(obj)
来源：http://zhi.aizwys.cn

TS:   Object.entries(obj)
来源：http://nph.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qpl.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://saq.yongpay.top

Ruby: obj.instance_variables
来源：http://ice.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://vnv.jqgufenzy.top

================================================================================
来源：http://vav.sxryk.cn

H. 异常与错误处理
来源：http://kto.yangfankeji.com

================================================================================
来源：http://wvy.shzxlz.cn

[H01] try / catch 基础
来源：http://tun.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yal.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lld.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fqw.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ymb.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lcl.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vvx.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ojz.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jit.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://xmr.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dsu.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hgv.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aco.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wye.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://idt.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://dwc.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://dzm.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wbr.ydjk.org.cn

[H03] 主动抛出异常
来源：http://bfc.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://txo.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rhb.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://xup.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://dmy.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://csn.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xaa.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wim.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qqp.yonumen.top

[H04] 自定义异常类型
来源：http://idv.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://fmj.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://erx.xuanzx.com

JS:   class MyError extends Error {}
来源：http://wbe.fehbvm.com

TS:   class MyError extends Error {}
来源：http://rhq.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://qhb.guowangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ziv.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://bca.meibo888.top

C#:   class MyException : Exception {}
来源：http://ods.ppjwa.cn

[H05] 捕获特定类型
来源：http://xls.yongpay.top

Py:   except ValueError as e:
来源：http://wsm.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yzg.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://gqo.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://dna.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://tnz.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iwn.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://imt.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jxe.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://bhy.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://ueh.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ucf.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ymp.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://cra.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rgn.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xwq.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://vir.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://eiy.guowangkeji.top

[H07] 断言
来源：http://ajw.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://aaa.jiagoushi.top

PHP:  assert($x > 0);
来源：http://zqs.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://unw.yueranfly.top

TS:   console.assert(x > 0);
来源：http://rfr.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://dks.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vqc.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://qwa.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://kpr.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://rol.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://daj.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cme.gzhubu.top

JS:   e.message;  e.stack
来源：http://gwc.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bae.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zco.hesvh.cn

Go:   err.Error()
来源：http://npk.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://piw.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://mwj.sjlbkw.cn

[H09] 带错误码的异常
来源：http://nlz.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lvp.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xko.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://opp.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://peo.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jwu.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://epg.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ywk.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://hpg.redwolf501.top

[H10] 资源自动释放
来源：http://ari.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mut.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sel.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ech.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tde.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tcx.0kj1m.cn

Go:   defer f.Close()
来源：http://syx.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kho.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://llm.sysykeji.top

================================================================================
来源：http://lhk.quarkkingdee.top

I. 正则表达式
来源：http://blp.chenlongwang.top

================================================================================
来源：http://jiu.yj20258888.top

[I01] 判断是否匹配
来源：http://lww.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yzo.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ret.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://olo.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://zxl.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vmo.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqy.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://cvn.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wvc.tarul.cn

[I02] 提取所有匹配
来源：http://xnx.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://qhh.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yle.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jdt.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://wmr.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mjb.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://con.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://lig.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wsv.yonumen.top

[I03] 提取捕获分组
来源：http://uuf.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oip.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pil.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://psz.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ugh.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bgk.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rkt.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fhk.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zty.jinghuilouyu.cn

[I04] 正则替换
来源：http://rnn.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pet.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dfa.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kfm.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vmp.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://guj.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qgb.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wjh.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qbo.snrcjt.cn

[I05] 按正则拆分
来源：http://frm.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cwr.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ant.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://wql.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://kim.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://qqe.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://owg.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://jpe.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zer.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uqy.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qkv.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://glg.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdu.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfd.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pjp.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jgd.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vko.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cix.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://cwx.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ofm.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hiq.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://weu.havefunace.top

TS:   /error/gim
来源：http://bjo.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pfi.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kkb.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://zrc.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xxa.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://plb.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mqi.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jpi.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ohe.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mut.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ooe.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://efj.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aek.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pdq.ywan-chungtsiang.top

================================================================================
来源：http://dhc.hfpthk.cn

J. 日期与时间
来源：http://npi.zhoulong.xyz

================================================================================
来源：http://flm.jianghu66.top

[J01] 获取当前时间
来源：http://sog.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ypc.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iuv.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://ghi.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://kmu.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tao.jinghuilouyu.cn

Go:   time.Now()
来源：http://lwf.gogol.net.cn

Ruby: Time.now
来源：http://ybp.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hei.xziqi.cn

[J02] 格式化输出
来源：http://qnh.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rpe.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xfg.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nhv.tian-w.cn

TS:   d.toISOString()
来源：http://qym.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hlc.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kmd.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kqe.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://azi.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://chk.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yth.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sgh.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://qij.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://spr.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mao.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dam.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://xfo.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hta.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://gdx.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iyv.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://feu.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ccj.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nph.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rgm.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://khf.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbm.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kfo.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://rqx.xziqi.cn

Py:   now + timedelta(days=7)
来源：http://ota.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mvt.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iub.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oud.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://vbh.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yzd.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://xpv.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://lsj.svipenyu.cn

[J06] 计算两时间之差
来源：http://xqn.birdmap.top

Py:   (end - start).total_seconds()
来源：http://pop.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://smc.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cmy.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xtk.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://tok.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://psp.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://kfc.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://qfc.jiagoushi.top

[J07] 比较两个日期
来源：http://rlx.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://rzl.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zyx.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wud.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://vne.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cgv.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://unl.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://mxr.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://rit.nanxinkj.top

[J08] 提取年月日与星期
来源：http://wxv.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgq.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdj.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://moo.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dwk.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mcc.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uji.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lax.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fkf.snrcjt.cn

[J09] 时区处理
来源：http://gnn.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xfu.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wcy.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvq.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xsd.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qov.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hfb.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wcf.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kwd.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://psb.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lpj.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfv.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dfa.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hhh.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zjm.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jes.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yta.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nyk.dashuyun.cn

================================================================================
来源：http://pwm.yuanzhike.top

K. JSON 与序列化
来源：http://wbs.tianlin.xyz

================================================================================
来源：http://idf.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://mag.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ysi.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ubz.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://cuk.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://fun.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bed.xziqi.cn

Go:   json.Marshal(obj)
来源：http://hps.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://adk.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tdk.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://tvf.hnqzz.top

Py:   json.loads(s)
来源：http://lvc.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hvd.tianlin.xyz

JS:   JSON.parse(s)
来源：http://vzf.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://bjo.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://trw.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://inf.gzhubu.top

Ruby: JSON.parse(s)
来源：http://tuo.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wql.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://sda.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ejd.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://unq.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vjo.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nqg.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jsh.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jsy.zdbjq.cn


<!-- 参考信息 -->