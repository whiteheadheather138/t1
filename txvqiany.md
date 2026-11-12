代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iao.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ojb.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://whe.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iwi.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://mdi.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qlk.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://dkp.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hfb.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://hnx.tarul.cn

JS:   Object.entries(obj)
来源：http://ufi.cdnleiting.top

TS:   Object.entries(obj)
来源：http://dck.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vty.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sdn.mhx1999.top

Ruby: obj.instance_variables
来源：http://tva.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://xvi.birdmap.top

================================================================================
来源：http://bku.yj20258888.top

H. 异常与错误处理
来源：http://qnl.fktsv.cn

================================================================================
来源：http://ukx.yj20258.top

[H01] try / catch 基础
来源：http://snv.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vnm.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gik.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rce.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://caw.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uwz.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xbg.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uxd.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rrk.jianghu66.top

[H02] finally / ensure 收尾
来源：http://amq.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://oxu.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhi.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ncw.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gdj.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://oon.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jyd.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ynt.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nds.mhx1999.top

[H03] 主动抛出异常
来源：http://aby.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://mnn.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sdw.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://flg.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://ghi.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mru.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dvo.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://goc.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://gui.jianghu66.top

[H04] 自定义异常类型
来源：http://gld.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://fmb.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://ihp.yuxming.cn

JS:   class MyError extends Error {}
来源：http://uyj.epnwcf.com

TS:   class MyError extends Error {}
来源：http://xxe.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://tyl.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zsm.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://awp.yvedp.cn

C#:   class MyException : Exception {}
来源：http://ado.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://qfm.iojbl.cn

Py:   except ValueError as e:
来源：http://zia.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://prd.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://vep.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ctn.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://sgj.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bqg.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://tkx.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ypi.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://pjw.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://rsx.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://sjr.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://zct.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://med.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jny.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kbp.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://djz.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://ehq.pycfn.com

[H07] 断言
来源：http://jdv.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://ngb.xinyue.icu

PHP:  assert($x > 0);
来源：http://pew.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://qfs.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://kia.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://uzz.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ato.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://nnt.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://ene.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://ivk.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://hsm.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mje.sufxvd.cn

JS:   e.message;  e.stack
来源：http://qgc.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qwb.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://aym.dianchejie.cn

Go:   err.Error()
来源：http://egk.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://zfq.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://dmv.fengsongda.top

[H09] 带错误码的异常
来源：http://zbk.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://awo.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://kbn.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dan.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpv.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mbw.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ink.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://klq.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://frf.gzhubu.top

[H10] 资源自动释放
来源：http://tkk.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rfe.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gni.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qqb.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pry.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tpf.pengpengdd.cyou

Go:   defer f.Close()
来源：http://sdt.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ugw.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bqo.hcnkem.com

================================================================================
来源：http://lzl.sysykeji.top

I. 正则表达式
来源：http://mix.jianghu66.top

================================================================================
来源：http://thn.yuxming.cn

[I01] 判断是否匹配
来源：http://wbh.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fjf.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://ufl.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://dzx.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://nkq.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gwq.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mgs.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://pgz.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vzr.shuidangran.top

[I02] 提取所有匹配
来源：http://fdu.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://imy.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://svj.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://haz.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://hfi.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dfn.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fvr.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://atu.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tdw.yongpay.top

[I03] 提取捕获分组
来源：http://gss.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tse.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rpc.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfx.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eqd.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oih.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eii.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ppc.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ybr.feifeiyinyue.top

[I04] 正则替换
来源：http://twd.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://agw.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sgt.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://fnx.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qtd.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://vfo.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bad.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cnd.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ehq.zhongyouzk.top

[I05] 按正则拆分
来源：http://ppr.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aiy.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gsv.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ias.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://npg.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://tdk.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mxf.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://uwf.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xcw.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uub.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dox.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://agx.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://quh.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dto.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pie.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rbs.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gmc.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kil.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://pfk.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xzu.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://csr.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xll.meibo888.top

TS:   /error/gim
来源：http://xhl.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dtq.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lvk.ivvv.top

Ruby: s.scan(/error/i)
来源：http://kxd.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yza.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://lwa.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jcy.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vwv.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://piw.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bzm.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://plz.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tbt.meibo888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://min.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hyv.jqgufenzy.top

================================================================================
来源：http://twk.yj20258888.top

J. 日期与时间
来源：http://yxt.hcnkem.com

================================================================================
来源：http://oey.pengpengdd.cyou

[J01] 获取当前时间
来源：http://irx.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fpr.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iof.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://vbh.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://hjw.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qkv.redwolf501.top

Go:   time.Now()
来源：http://ply.tanke756.top

Ruby: Time.now
来源：http://aei.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dzt.chenzaomai.com

[J02] 格式化输出
来源：http://uvk.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jnc.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ezy.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dcl.sjlbkw.cn

TS:   d.toISOString()
来源：http://kfu.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fcu.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hek.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tiq.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ojp.smart0.xyz

[J03] 字符串解析为日期
来源：http://tay.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mbw.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://phd.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://wrn.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://qrg.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://gnr.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uwu.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://lnx.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://voe.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://rbj.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cdg.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://agu.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://svn.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ife.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dbh.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbb.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zsz.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xwd.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://yam.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://hla.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gsi.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejl.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ham.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://sym.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://apv.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://duf.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://bwi.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://yzd.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://hgz.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://hwt.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rvy.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gvm.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://ukh.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://clk.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://idi.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://pho.yj202588.top

[J07] 比较两个日期
来源：http://fjw.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://oqp.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gzq.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://mnb.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://nsl.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://erm.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://whg.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rqe.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://fqe.andypj.xyz

[J08] 提取年月日与星期
来源：http://zxu.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://esr.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sng.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rou.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://afx.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cjs.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ois.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cvm.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iqr.snrcjt.cn

[J09] 时区处理
来源：http://qta.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wdn.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xou.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nin.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxf.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://esg.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mah.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wio.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rin.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://wqi.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kmj.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gqj.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://neu.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jqd.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nhs.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ken.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzc.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zqh.bjfxy.top

================================================================================
来源：http://irp.aibaodan.cn

K. JSON 与序列化
来源：http://pcf.pengpengdd.cyou

================================================================================
来源：http://acd.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://cdp.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wlb.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rvs.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://lhu.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://cwc.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yym.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://oiu.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://ovi.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uve.hesvh.cn

[K02] JSON 字符串转对象
来源：http://moh.pycfn.com

Py:   json.loads(s)
来源：http://xol.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ryg.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://gvu.gzhubu.top

TS:   JSON.parse(s)
来源：http://rkb.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lew.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://fwz.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://pzk.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mbv.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://vuu.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bky.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sjj.fanxiaobao.xyz


<!-- 参考信息 -->