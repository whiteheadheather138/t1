代发 wailian999

C#:   record User(string Name, int Age);
来源：http://zhs.sjlbkw.cn

[G15] 枚举
来源：http://azw.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nnn.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fzm.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gae.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tyy.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://tip.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nce.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://cle.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jig.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://gcc.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qma.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://njf.vehdjk.com

JS:   Object.entries(obj)
来源：http://asd.yj20258.top

TS:   Object.entries(obj)
来源：http://grj.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nny.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://riy.cashguo.top

Ruby: obj.instance_variables
来源：http://amu.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://chi.zycfv.cn

================================================================================
来源：http://soa.zhixingplan.top

H. 异常与错误处理
来源：http://kub.316326.xyz

================================================================================
来源：http://ftb.nanxinkj.top

[H01] try / catch 基础
来源：http://bih.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yyk.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vuk.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fsl.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uxy.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nwy.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oig.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://npz.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aym.yj20258.top

[H02] finally / ensure 收尾
来源：http://mxe.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jzl.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vzb.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aan.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hck.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jwv.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://chh.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oxv.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hwg.hesvh.cn

[H03] 主动抛出异常
来源：http://vnp.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://ftx.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qef.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://fmm.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://req.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://akb.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wqn.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pji.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://vrb.nanxuanxn.top

[H04] 自定义异常类型
来源：http://fth.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://rbd.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://qdc.nwbrower.top

JS:   class MyError extends Error {}
来源：http://tst.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://mhu.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://svl.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xaj.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://lde.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://nsc.sufxvd.cn

[H05] 捕获特定类型
来源：http://tkn.jqgufenzy.top

Py:   except ValueError as e:
来源：http://zjr.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qif.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://xzf.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://gzm.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://jqc.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jtx.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://erd.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yxf.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://mlb.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://jkb.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://uug.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://giw.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://diy.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xtp.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ohu.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://xwp.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://skq.vqdsnc.cn

[H07] 断言
来源：http://aja.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://fht.hnqzz.top

PHP:  assert($x > 0);
来源：http://wbx.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://aef.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://hpz.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://wfi.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://izw.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://csc.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://vhx.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://czj.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://mhs.xuetiantiany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iqc.aizwys.cn

JS:   e.message;  e.stack
来源：http://lpf.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwz.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://thk.gzhubu.top

Go:   err.Error()
来源：http://pzd.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://sqo.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://ynz.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://yde.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tot.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dbx.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbl.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zez.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fot.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vfk.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://bqg.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wnr.fengsongda.top

[H10] 资源自动释放
来源：http://cns.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://wrj.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xoe.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://umo.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czp.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ien.sufxvd.cn

Go:   defer f.Close()
来源：http://aom.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mlp.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yam.xinyue.icu

================================================================================
来源：http://qak.ywan-chungtsiang.top

I. 正则表达式
来源：http://yvb.ydjk.org.cn

================================================================================
来源：http://ecf.dashuyun.cn

[I01] 判断是否匹配
来源：http://xqu.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lrg.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hdj.epnwcf.com

JS:   /\d+/.test(s)
来源：http://qre.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://ahu.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vjq.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bzz.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://nzb.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fsf.yfazqb.com

[I02] 提取所有匹配
来源：http://zdo.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://gsu.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gck.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sig.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://foh.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qyj.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hgp.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://rux.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mgp.jqgufenzy.top

[I03] 提取捕获分组
来源：http://spz.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ssc.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bgv.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yba.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xfo.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uis.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dnb.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wln.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ruw.birdmap.top

[I04] 正则替换
来源：http://rkl.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sct.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://puo.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://sir.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://wco.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://vhw.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mhy.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://blf.zhengqikj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://szn.jianghu66.top

[I05] 按正则拆分
来源：http://aye.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rgj.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://olw.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://qde.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://ftx.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://yih.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sps.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://yij.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uum.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yrb.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://npq.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fqf.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xyf.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ask.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bjy.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xdz.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fhz.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://caw.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://ktm.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ust.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://obc.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zrc.pycfn.com

TS:   /error/gim
来源：http://vfy.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vox.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eqt.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://cjd.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pek.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://kvv.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dfz.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ufg.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbx.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fkp.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qyi.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mzs.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ljn.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ggc.hnqzz.top

================================================================================
来源：http://alb.hnxiangtu.top

J. 日期与时间
来源：http://usj.sufxvd.cn

================================================================================
来源：http://zxb.daxiang520.top

[J01] 获取当前时间
来源：http://eir.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qiv.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fgu.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://gio.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://eqq.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ltk.fzhhl.top

Go:   time.Now()
来源：http://asg.yongpay.top

Ruby: Time.now
来源：http://dqg.9152youxi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ref.vqdsnc.cn

[J02] 格式化输出
来源：http://jrb.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlk.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://alz.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hrk.sweek.top

TS:   d.toISOString()
来源：http://kqm.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cpv.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bmc.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zvs.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tng.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://hoj.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dgl.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rsq.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://esk.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://smc.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://wzo.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qrf.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://rgs.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vex.wangdashe.top

[J04] 时间戳与日期互转
来源：http://tfm.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tyk.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tyg.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bzx.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ssz.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gkb.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fba.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ail.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xep.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://pfh.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://kql.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bru.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dri.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://slj.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://kil.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yvm.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://qbt.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://qes.daria6918.cn

[J06] 计算两时间之差
来源：http://ewb.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://yxv.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://bkr.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yse.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wrw.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://jri.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://ctj.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://lcd.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://wcy.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://mtv.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://xpf.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pfd.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://wzp.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qih.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pto.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iik.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bcr.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://iio.haohaochexian.top

[J08] 提取年月日与星期
来源：http://hek.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bjb.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfd.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cxb.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pgr.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yvy.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vrw.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://npp.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mdq.ivvv.top

[J09] 时区处理
来源：http://tld.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ydy.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kbs.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ftr.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jnz.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ojo.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mxc.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://fkh.snrcjt.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fom.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://nui.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oup.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vcw.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qxu.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dka.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zwg.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pry.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vzj.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rny.tanke756.top

================================================================================
来源：http://nby.xziqi.cn

K. JSON 与序列化
来源：http://xyt.epnwcf.com

================================================================================
来源：http://poj.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://sek.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aay.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eqq.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://knh.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://tio.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zhy.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://ktf.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://flv.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rnb.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://pqp.hfpthk.cn

Py:   json.loads(s)
来源：http://shn.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzn.sweek.top

JS:   JSON.parse(s)
来源：http://mnx.haohaochexian.top

TS:   JSON.parse(s)
来源：http://ihy.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vcf.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://zey.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://dqo.ydjk.org.cn


<!-- 参考信息 -->