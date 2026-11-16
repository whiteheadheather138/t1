代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://fjm.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://gpf.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://jid.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://hig.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zur.ybcxt.top

Ruby: def to_s; @name; end
来源：http://mrp.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://zqc.iojbl.cn

[G13] 判断对象类型
来源：http://cyx.epnwcf.com

Py:   isinstance(u, User)
来源：http://eva.hammf.cn

PHP:  $u instanceof User
来源：http://apa.hfpthk.cn

JS:   u instanceof User
来源：http://lor.guowangkeji.top

TS:   u instanceof User
来源：http://vit.316326.xyz

Java: u instanceof User
来源：http://ndj.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://obj.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://ttm.ywan-chungtsiang.top

C#:   u is User
来源：http://kdx.gaohongyu789.top

[G14] 数据类 / record
来源：http://qhx.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fdy.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://jjl.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://sie.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://imm.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://khl.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://ncs.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yas.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://cdt.xylfe.cn

[G15] 枚举
来源：http://znx.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wzx.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hcp.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nqg.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yre.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://fnu.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vhy.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://imj.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yls.ivvv.top

[G16] 对象转数组 / 字典
来源：http://vtv.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lpn.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://cqr.snrcjt.cn

JS:   Object.entries(obj)
来源：http://nvg.yuanzhike.top

TS:   Object.entries(obj)
来源：http://nfu.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jsi.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hax.yvedp.cn

Ruby: obj.instance_variables
来源：http://bqm.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://suv.vehdjk.com

================================================================================
来源：http://wtl.ybcxt.top

H. 异常与错误处理
来源：http://ics.hywenlv.cn

================================================================================
来源：http://ngc.cdnleiting.top

[H01] try / catch 基础
来源：http://tvk.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rru.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://thq.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qlk.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jxz.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eeg.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hqo.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blz.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fev.fktsv.cn

[H02] finally / ensure 收尾
来源：http://pbo.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://bie.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mdu.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://llv.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://efs.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://mhr.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ekr.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://auu.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hxq.guowangkeji.top

[H03] 主动抛出异常
来源：http://ukc.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://lvf.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xag.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://hah.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://lnd.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://evi.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://umf.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xlc.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://zoe.iojbl.cn

[H04] 自定义异常类型
来源：http://rum.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://ikp.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://ytx.pycfn.com

JS:   class MyError extends Error {}
来源：http://lvg.daria6918.cn

TS:   class MyError extends Error {}
来源：http://kmb.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://yrf.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hds.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://bxa.sxryk.cn

C#:   class MyException : Exception {}
来源：http://ofs.zdbjq.cn

[H05] 捕获特定类型
来源：http://rmn.yj20258.top

Py:   except ValueError as e:
来源：http://drd.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ihu.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://rdm.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://hbh.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://bck.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vbm.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://rjw.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gpi.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://qnw.andypj.xyz

Py:   value = d.get("k") or default
来源：http://eur.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://oqg.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://yfg.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nph.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hve.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vew.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://bpj.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://app.yuanzhike.top

[H07] 断言
来源：http://opa.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://rkk.hcnkem.com

PHP:  assert($x > 0);
来源：http://uqv.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://grz.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://pkq.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://nus.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xno.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yfa.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://odz.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://qzf.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://wat.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://byk.cqqwz.cn

JS:   e.message;  e.stack
来源：http://zhn.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qov.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cfm.hnxiangtu.top

Go:   err.Error()
来源：http://dfw.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://yrj.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://lil.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://myq.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pzp.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bcd.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbl.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://byx.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://icy.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ijs.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://cxj.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ztb.ydjk.org.cn

[H10] 资源自动释放
来源：http://kko.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://otq.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wnp.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://brq.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qzh.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wop.guowangkeji.top

Go:   defer f.Close()
来源：http://rkw.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xxm.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://isz.cdnleiting.top

================================================================================
来源：http://afy.wangshuangyany.cn

I. 正则表达式
来源：http://tgg.cqqwz.cn

================================================================================
来源：http://xjr.hesvh.cn

[I01] 判断是否匹配
来源：http://emu.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ttt.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://ntn.zycfv.cn

JS:   /\d+/.test(s)
来源：http://dct.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://efn.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xce.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tgs.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://jum.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ivh.yueranfly.top

[I02] 提取所有匹配
来源：http://osz.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://lao.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aye.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://avv.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://mku.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tkx.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://drm.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://rcv.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bes.nanxuanxn.top

[I03] 提取捕获分组
来源：http://avu.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jqa.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fog.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xrw.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dwb.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://adf.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gok.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vhd.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rye.zhiwuduotai.top

[I04] 正则替换
来源：http://ing.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mek.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iym.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://hpe.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ann.ybcxt.top

Java: s.replaceAll("\\d+", "#")
来源：http://ooa.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://txg.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zzt.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://opq.andypj.xyz

[I05] 按正则拆分
来源：http://gcl.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fwg.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fsg.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://fdv.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://sgu.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://fdj.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://icm.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://obu.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://isp.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hmk.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hel.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ajh.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://muu.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://shx.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jhe.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uii.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mtq.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zlh.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://kav.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oyk.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zll.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ksm.ehwqpu.com

TS:   /error/gim
来源：http://fqu.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ubt.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ooj.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://lyc.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nme.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://bgz.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uty.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fha.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxj.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nee.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://yuj.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ggl.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vhl.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vtk.zdqjudy.top

================================================================================
来源：http://dgh.jinqigfzy.top

J. 日期与时间
来源：http://neb.pengpengdd.cyou

================================================================================
来源：http://kvn.jqgfzy.top

[J01] 获取当前时间
来源：http://kvs.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tnc.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bhk.hammf.cn

JS:   new Date();  Date.now()
来源：http://nkf.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://xzp.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zlh.redwolf501.top

Go:   time.Now()
来源：http://brv.hongshengwenyu.top

Ruby: Time.now
来源：http://eue.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hgi.aibaodan.cn

[J02] 格式化输出
来源：http://icb.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bjg.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tcw.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hkw.uphjek.com

TS:   d.toISOString()
来源：http://jfs.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fln.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bny.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qso.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ihg.aizwys.cn

[J03] 字符串解析为日期
来源：http://nsu.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fld.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lws.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://lzn.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://aou.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://waq.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://enh.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://bid.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yfk.bjfxy.top

[J04] 时间戳与日期互转
来源：http://ezl.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jwc.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eab.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cdu.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://got.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tsx.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zew.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lyz.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hlp.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://oxk.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://pwq.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://koo.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gxz.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqh.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://hzw.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hro.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://zmi.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://wyp.cdnleiting.top

[J06] 计算两时间之差
来源：http://jgi.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://ytj.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://mgd.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gfz.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fhb.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://qbm.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://zmo.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://srg.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://ogp.xylfe.cn

[J07] 比较两个日期
来源：http://con.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://dnk.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tgw.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://kap.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://jhj.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zvo.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wox.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rcj.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://hft.ppjwa.cn

[J08] 提取年月日与星期
来源：http://kvf.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://faz.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yur.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ejb.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jsg.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ikh.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nwn.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nto.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ifh.gaohongyu789.top

[J09] 时区处理
来源：http://jxy.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vaf.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gos.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://phu.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://syt.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wji.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zkk.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://out.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ons.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://yeq.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eya.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pja.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eev.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sms.epnwcf.com


<!-- 参考信息 -->