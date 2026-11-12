代发 wailian999

C#:   record User(string Name, int Age);
来源：http://ibb.tianlin.xyz

[G15] 枚举
来源：http://vcz.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://saq.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sts.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kha.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ten.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://vsa.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ntt.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://ton.chenlongwang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ijr.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://doo.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xei.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://ywp.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://zhj.aibaodan.cn

TS:   Object.entries(obj)
来源：http://jrc.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qbh.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xxx.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://zoo.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://gfr.gotoacloud.top

================================================================================
来源：http://kjh.wangdashe.top

H. 异常与错误处理
来源：http://zlm.sysykeji.top

================================================================================
来源：http://hrq.jiagoushi.top

[H01] try / catch 基础
来源：http://mnb.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iam.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fct.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nyn.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zrp.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://don.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zix.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jmu.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dhr.nwbrower.top

[H02] finally / ensure 收尾
来源：http://isq.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bon.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xxb.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://nlx.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://foy.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://xod.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://nry.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wor.ehwqpu.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://mhw.tian-w.cn

[H03] 主动抛出异常
来源：http://uwy.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://xgo.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nxj.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://jxo.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://xks.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://uur.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://igc.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xgp.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wbm.hysaishi.cn

[H04] 自定义异常类型
来源：http://xin.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://mte.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://hnz.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://jcp.wangdashe.top

TS:   class MyError extends Error {}
来源：http://xjh.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://yjt.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wge.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://raf.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://lvu.ybcxt.top

[H05] 捕获特定类型
来源：http://ubf.jqgfzy.top

Py:   except ValueError as e:
来源：http://owl.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://znk.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://mar.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://gkk.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://tjd.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zii.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://rby.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jkv.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://ibi.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://val.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://frs.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nai.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://een.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jdx.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uin.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://jnj.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://ath.redwolf501.top

[H07] 断言
来源：http://zgq.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://gof.52xcode.cn

PHP:  assert($x > 0);
来源：http://qid.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://ctt.sweek.top

TS:   console.assert(x > 0);
来源：http://wtk.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://dfy.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bay.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://jlf.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://cll.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://lwh.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://awz.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kea.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://btv.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dyq.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qhw.pycfn.com

Go:   err.Error()
来源：http://auj.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://jgd.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://kls.cheryme.top

[H09] 带错误码的异常
来源：http://zdg.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hzu.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://hrz.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tbi.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ttj.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fiy.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aob.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://whi.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kfn.yangfankeji.com

[H10] 资源自动释放
来源：http://ths.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://uuc.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jmf.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hxr.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://boa.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wug.zdbjq.cn

Go:   defer f.Close()
来源：http://lmw.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vtw.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zde.jinghuilouyu.cn

================================================================================
来源：http://zoe.yj20258.top

I. 正则表达式
来源：http://kde.ivvv.top

================================================================================
来源：http://fjw.zhongyouzk.top

[I01] 判断是否匹配
来源：http://gxo.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uem.jqgfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://dou.fktsv.cn

JS:   /\d+/.test(s)
来源：http://cnj.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://rja.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eqg.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zkz.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://vue.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qxm.zhoulong.xyz

[I02] 提取所有匹配
来源：http://xic.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://jrk.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://caa.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rsu.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://pud.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dra.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ryq.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://lub.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fsi.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://vbp.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gno.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bzc.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ytg.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fre.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hnf.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eqg.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lhd.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zcn.fehbvm.com

[I04] 正则替换
来源：http://rsn.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fxk.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lsx.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://zaj.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rop.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://lfi.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ljj.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ivx.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bfy.zhengqikj.top

[I05] 按正则拆分
来源：http://roq.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nbr.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wuu.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://jnr.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://xwt.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://prw.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wzm.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://jhy.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nfg.jinghuilouyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://chg.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ava.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hzj.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nhw.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vui.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uhq.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xuu.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zyk.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oat.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://jsw.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dux.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bbq.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tpw.guannengcc.top

TS:   /error/gim
来源：http://umo.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dvj.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://puj.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://tpv.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xnr.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://blo.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yen.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cky.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfy.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xum.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pyy.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wuo.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ciw.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://esf.jinqigufen.top

================================================================================
来源：http://txg.haohaochexian.top

J. 日期与时间
来源：http://ikd.nanxinkj.top

================================================================================
来源：http://ccd.guannengcc.top

[J01] 获取当前时间
来源：http://mvk.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kqw.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vwh.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://dcq.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://qxk.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pml.ydzc1.top

Go:   time.Now()
来源：http://ska.shzxlz.cn

Ruby: Time.now
来源：http://nxo.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ugg.gaohongyu789.top

[J02] 格式化输出
来源：http://trx.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://seg.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://per.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vgn.iojbl.cn

TS:   d.toISOString()
来源：http://qgl.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tev.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://opb.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hdw.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://clz.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://erg.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dfm.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nfy.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://nib.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://nyn.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://tkc.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qvw.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://gbc.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nip.ivvv.top

[J04] 时间戳与日期互转
来源：http://thn.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iff.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vgd.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rvo.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fzj.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iht.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jlz.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ifu.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mzc.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://uax.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://zmx.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bbw.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nnm.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgz.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://pva.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eri.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://vwy.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://uqf.redwolf501.top

[J06] 计算两时间之差
来源：http://bfy.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://yix.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://ieb.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ejs.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fve.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://ugy.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://uuz.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://kzq.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://rsz.chenzaomai.com

[J07] 比较两个日期
来源：http://hqt.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://rtd.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ssy.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://njm.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://jbp.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owh.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gao.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://bat.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://pek.shuidangran.top

[J08] 提取年月日与星期
来源：http://tgd.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sho.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mcj.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gwj.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sdi.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://woz.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rpg.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qej.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lsn.yueranfly.top

[J09] 时区处理
来源：http://ahy.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gus.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fsd.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hku.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xnk.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cyu.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jji.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://trn.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://onu.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://xiy.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nya.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://umc.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qvf.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://avt.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://osf.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://edo.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ipo.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vel.tarul.cn

================================================================================
来源：http://hcg.pycfn.com

K. JSON 与序列化
来源：http://ojj.sysykeji.top

================================================================================
来源：http://oav.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://jbt.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uav.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ade.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://ubt.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://lkg.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uoc.smart0.xyz

Go:   json.Marshal(obj)
来源：http://bhr.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uja.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bke.bjfxy.top

[K02] JSON 字符串转对象
来源：http://zub.haohaochexian.top

Py:   json.loads(s)
来源：http://aoy.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://adk.ctjpmb.com

JS:   JSON.parse(s)
来源：http://czj.guannengcc.top

TS:   JSON.parse(s)
来源：http://glk.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzx.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://puz.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://xxb.0kj1m.cn


<!-- 参考信息 -->