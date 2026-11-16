代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hoy.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hpj.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://rre.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gac.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://kox.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uiz.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://rzd.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kff.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://ary.aizwys.cn

JS:   Object.entries(obj)
来源：http://vsv.havefunace.top

TS:   Object.entries(obj)
来源：http://sir.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://prk.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ygu.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://pco.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://tbn.0kj1m.cn

================================================================================
来源：http://xbv.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://hes.jiagoushi.top

================================================================================
来源：http://hsw.jinqigfzy.top

[H01] try / catch 基础
来源：http://dqp.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rfu.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uon.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tky.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rja.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jaw.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bcu.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qgt.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pvf.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://zbi.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://urs.jianghu66.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://thj.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bpm.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://urg.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://rtv.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xym.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://apq.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://smv.hcnkem.com

[H03] 主动抛出异常
来源：http://exv.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://lwd.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ckh.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://uvk.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://ptf.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mky.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nuz.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rlc.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://pca.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://thg.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://gpo.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://mmu.redwolf501.top

JS:   class MyError extends Error {}
来源：http://nkv.fengsongda.top

TS:   class MyError extends Error {}
来源：http://ybf.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://gux.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vjn.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://wkx.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://tks.gotoacloud.top

[H05] 捕获特定类型
来源：http://pbp.yj20258.top

Py:   except ValueError as e:
来源：http://fej.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lhp.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://gsa.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://hdb.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://gcf.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dyc.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://ezs.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lwk.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://sbj.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://bfx.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rax.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xox.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://din.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dyq.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fth.gotoacloud.top

Ruby: d&.dig(:a, :b)
来源：http://kea.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://zsk.0kj1m.cn

[H07] 断言
来源：http://ieo.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://xwg.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://uul.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://ruz.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://ldm.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://bda.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://azk.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://kok.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://mmw.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://qjz.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://tnh.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xkw.hywenlv.cn

JS:   e.message;  e.stack
来源：http://fzp.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qoz.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://khe.yuanzhike.top

Go:   err.Error()
来源：http://fkh.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://tvy.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://gtj.sjlbkw.cn

[H09] 带错误码的异常
来源：http://lxb.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://luo.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kwv.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ruv.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://abs.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eoe.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pdm.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://biu.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ioj.tian-w.cn

[H10] 资源自动释放
来源：http://vek.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lrj.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zbd.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pkh.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ldp.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://urr.iojbl.cn

Go:   defer f.Close()
来源：http://ezk.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rgp.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nwh.ydzc1.top

================================================================================
来源：http://vab.dashuyun.cn

I. 正则表达式
来源：http://yuu.daria6918.cn

================================================================================
来源：http://dgs.hywenlv.cn

[I01] 判断是否匹配
来源：http://qmd.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wyd.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://mgv.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://adn.yj202588.top

TS:   /\d+/.test(s)
来源：http://rmf.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bhd.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ghm.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://hbk.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://deu.hysaishi.cn

[I02] 提取所有匹配
来源：http://ngl.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://btc.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://flp.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mhn.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://ang.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://reb.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://atr.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://qpl.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://azs.guowangkeji.top

[I03] 提取捕获分组
来源：http://fcz.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tqp.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zst.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ehp.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xtm.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yzz.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pkn.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pmw.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lqz.shangyingyoupin.top

[I04] 正则替换
来源：http://hck.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://iwz.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://koa.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://uyh.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://smo.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://xmh.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://prw.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hne.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://swk.yuanzhike.top

[I05] 按正则拆分
来源：http://mhm.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vnh.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xgv.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://jpl.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://fdi.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://rgh.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pjo.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://ozr.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://brs.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://anv.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sia.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uob.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://buk.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sam.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xbv.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nkx.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ojs.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://djq.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://lxm.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ugn.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mgb.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rtu.yj20258888.top

TS:   /error/gim
来源：http://rya.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://seu.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ege.cheryme.top

Ruby: s.scan(/error/i)
来源：http://ity.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gvh.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://qbr.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://juq.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://krc.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dnw.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lay.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bmj.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ibq.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xgv.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ezu.chenjidiqi.icu

================================================================================
来源：http://clj.yanxiufei.cn

J. 日期与时间
来源：http://jsm.hysaishi.cn

================================================================================
来源：http://gxy.yonumen.top

[J01] 获取当前时间
来源：http://hfh.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://yyy.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nfb.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://wib.wangdashe.top

TS:   new Date();  Date.now()
来源：http://ufy.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zff.yj202588.top

Go:   time.Now()
来源：http://vgb.jlsjyb.cn

Ruby: Time.now
来源：http://gip.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xdg.birdmap.top

[J02] 格式化输出
来源：http://qcq.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mbx.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lzj.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qcg.ctjpmb.com

TS:   d.toISOString()
来源：http://ivd.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://inl.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://skj.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gif.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://djk.shuidangran.top

[J03] 字符串解析为日期
来源：http://iyc.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dvi.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ixz.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://ppr.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://gpv.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yvc.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wca.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://zth.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qli.cheryme.top

[J04] 时间戳与日期互转
来源：http://svm.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pgh.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uws.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxb.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bpl.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uyv.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rrn.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ude.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vjp.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://fmv.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://unm.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oqb.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wyb.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qeb.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://lkb.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vao.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://pgi.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://jla.gotoacloud.top

[J06] 计算两时间之差
来源：http://vzg.yj20258.top

Py:   (end - start).total_seconds()
来源：http://hke.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://bug.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rho.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bhf.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://kzg.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://npz.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://iqi.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://gcp.uphjek.com

[J07] 比较两个日期
来源：http://xab.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://sgo.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rvu.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://myw.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ntt.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pzz.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vsd.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://xpg.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://nqm.9152youxi.cn

[J08] 提取年月日与星期
来源：http://kws.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tlf.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dmp.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tfh.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rct.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gbr.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lqn.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ehm.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sxk.sufxvd.cn

[J09] 时区处理
来源：http://oen.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zag.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jkj.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rka.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://teu.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjn.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zeo.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mhb.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wkw.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://jwx.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://doc.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xbx.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vlc.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fhx.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hea.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ebf.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wxa.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wpi.meibo888.top

================================================================================
来源：http://sri.birdmap.top

K. JSON 与序列化
来源：http://heh.gaohongyu789.top

================================================================================
来源：http://gie.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://dux.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://niw.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ufr.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://exb.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://zqj.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://auk.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://ayi.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vnl.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bxm.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://dcz.ivvv.top

Py:   json.loads(s)
来源：http://gor.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://onj.hnqzz.top

JS:   JSON.parse(s)
来源：http://ihs.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://nuu.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jlm.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://pxd.hammf.cn

Ruby: JSON.parse(s)
来源：http://qgu.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://amy.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://dtm.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tta.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://inq.wangdashe.top


<!-- 参考信息 -->