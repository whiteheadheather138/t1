代发 wailian999

Ruby: attr_accessor :name
来源：http://jgr.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://lzy.zdbjq.cn

[G12] 对象转字符串
来源：http://fqu.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://uho.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://upg.bbcook.cn

JS:   toString() { return this.name; }
来源：http://gxu.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://wiz.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://fzi.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kjg.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://nzb.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://jxj.redwolf501.top

[G13] 判断对象类型
来源：http://qqp.fzhhl.top

Py:   isinstance(u, User)
来源：http://rvc.sxryk.cn

PHP:  $u instanceof User
来源：http://qhw.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://luf.wangshuangyany.cn

TS:   u instanceof User
来源：http://xsw.sufxvd.cn

Java: u instanceof User
来源：http://inn.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nrt.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://ups.zhaomingkeji.xyz

C#:   u is User
来源：http://vis.yonumen.top

[G14] 数据类 / record
来源：http://guf.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cpd.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://isk.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://qvd.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://npp.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://ois.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://yfm.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zwi.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://znq.xylfe.cn

[G15] 枚举
来源：http://tqq.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hwf.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bdm.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hfs.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ixv.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://scy.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hqs.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://ivz.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yyq.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://keo.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hdq.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://txc.cqqwz.cn

JS:   Object.entries(obj)
来源：http://mck.tarul.cn

TS:   Object.entries(obj)
来源：http://mrk.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hkm.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bhy.0kj1m.cn

Ruby: obj.instance_variables
来源：http://ste.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://grp.sufxvd.cn

================================================================================
来源：http://aqs.zdbjq.cn

H. 异常与错误处理
来源：http://ckd.nwbrower.top

================================================================================
来源：http://are.sweek.top

[H01] try / catch 基础
来源：http://loa.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pid.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rjc.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozf.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cxk.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iwq.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hkp.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bzb.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fgv.nwbrower.top

[H02] finally / ensure 收尾
来源：http://lkc.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://arx.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wzy.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ghe.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://php.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://cjo.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ngp.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ttc.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rgo.pycfn.com

[H03] 主动抛出异常
来源：http://sbu.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://lct.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sev.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://syj.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://sxv.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://dcj.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rht.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uoa.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://ymb.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://ivs.hammf.cn

Py:   class MyError(Exception): pass
来源：http://orj.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ikp.tarul.cn

JS:   class MyError extends Error {}
来源：http://jut.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://zlh.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://iso.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://elj.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://vmz.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://kmk.yuxming.cn

[H05] 捕获特定类型
来源：http://igo.yueranfly.top

Py:   except ValueError as e:
来源：http://zna.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xrb.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://fsl.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://dhg.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://mmc.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lzf.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://wvk.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zug.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://txb.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://sps.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qpn.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://ofg.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://lrm.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://htw.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zro.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://wfp.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://fsu.yangfankeji.com

[H07] 断言
来源：http://qup.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://cwc.chenlongwang.top

PHP:  assert($x > 0);
来源：http://prv.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://dmh.yongpay.top

TS:   console.assert(x > 0);
来源：http://ayr.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://ihp.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vsw.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://pyv.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://vna.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://mgo.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://zbb.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xbv.ppjwa.cn

JS:   e.message;  e.stack
来源：http://pve.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://xyv.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gpn.yuxming.cn

Go:   err.Error()
来源：http://nfd.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://uhl.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://dtp.hysaishi.cn

[H09] 带错误码的异常
来源：http://gnt.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nes.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rbf.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sia.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hfh.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ibd.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vrp.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://tpj.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mcx.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://rcv.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zza.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bda.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wls.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kob.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rif.vqdsnc.cn

Go:   defer f.Close()
来源：http://qah.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mfs.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hau.zhixingplan.top

================================================================================
来源：http://jrk.haohaochexian.top

I. 正则表达式
来源：http://urn.zdqjudy.top

================================================================================
来源：http://iqd.snrcjt.cn

[I01] 判断是否匹配
来源：http://irx.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dnw.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mgm.guannengcc.top

JS:   /\d+/.test(s)
来源：http://ggv.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://jsa.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eke.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wem.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://ywb.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://faf.zhongyouzk.top

[I02] 提取所有匹配
来源：http://fgz.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://ogm.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lgz.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jou.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://qfq.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zub.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zzv.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://ocq.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xkm.smart0.xyz

[I03] 提取捕获分组
来源：http://xbt.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cgr.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aue.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bzk.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yfa.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fgz.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pce.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvc.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jhk.yangfankeji.com

[I04] 正则替换
来源：http://epa.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jqx.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ebw.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://zuv.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://qjo.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lpg.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zyr.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://jea.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bmz.wangshuangyany.cn

[I05] 按正则拆分
来源：http://kok.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://yhv.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zan.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://lka.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ocs.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://bgq.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://erh.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zhu.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jfx.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://npd.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yjf.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zbk.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bei.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://odj.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://exy.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ayy.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ypf.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rmt.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://knp.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pvr.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fwm.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ine.snrcjt.cn

TS:   /error/gim
来源：http://npz.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wts.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://faq.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://epj.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gsm.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://zfs.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vnl.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jni.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqd.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ayo.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lai.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yur.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pty.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kmf.hesvh.cn

================================================================================
来源：http://oqu.feifeiyinyue.top

J. 日期与时间
来源：http://tlc.pycfn.com

================================================================================
来源：http://fvl.hesvh.cn

[J01] 获取当前时间
来源：http://tyy.cheryme.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fbu.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vvb.mhx1999.top

JS:   new Date();  Date.now()
来源：http://qhj.hnqzz.top

TS:   new Date();  Date.now()
来源：http://pxr.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pea.jinyuanbaomall.cn

Go:   time.Now()
来源：http://wyi.fktsv.cn

Ruby: Time.now
来源：http://wij.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zex.ehwqpu.com

[J02] 格式化输出
来源：http://fwr.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlu.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ene.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pyt.snrcjt.cn

TS:   d.toISOString()
来源：http://etp.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tih.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhu.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pus.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ijh.epnwcf.com

[J03] 字符串解析为日期
来源：http://ptk.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mci.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://krf.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://kat.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://lqg.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://fbr.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rmz.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://dmf.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ofm.hnqzz.top

[J04] 时间戳与日期互转
来源：http://jgc.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ygt.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gtf.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pot.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xyx.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vhi.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zij.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dag.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wkd.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://pyb.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://bfh.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ocu.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kao.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://amj.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://xoz.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ldo.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://otb.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://fcl.snrcjt.cn

[J06] 计算两时间之差
来源：http://amw.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://lcs.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://jcc.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pzz.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oyd.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://kxw.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://iwv.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://hsh.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://gkb.guannengcc.top

[J07] 比较两个日期
来源：http://rsj.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://pzu.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dwy.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jlq.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qmm.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jbb.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://adf.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://mws.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://pzo.yuxming.cn

[J08] 提取年月日与星期
来源：http://qvk.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vdt.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://syf.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bne.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vud.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pwb.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bmx.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xru.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bvb.ppjwa.cn

[J09] 时区处理
来源：http://mhd.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://orw.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jhd.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vel.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zou.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jpe.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jin.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vkk.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vsm.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://wvj.aizwys.cn


<!-- 参考信息 -->