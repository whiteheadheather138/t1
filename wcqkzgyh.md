代发 wailian999

Ruby: attr_accessor :name
来源：http://mmi.bjfxy.top

C#:   public string Name { get; set; }
来源：http://waj.gotoacloud.top

[G12] 对象转字符串
来源：http://qrk.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://ovq.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jqk.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://aak.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://tjh.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://cml.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rqz.tian-w.cn

Ruby: def to_s; @name; end
来源：http://uhf.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://iga.epnwcf.com

[G13] 判断对象类型
来源：http://oew.daria6918.cn

Py:   isinstance(u, User)
来源：http://are.yj20258888.top

PHP:  $u instanceof User
来源：http://ugl.wangdashe.top

JS:   u instanceof User
来源：http://afz.pengpengdd.cyou

TS:   u instanceof User
来源：http://arw.hcnkem.com

Java: u instanceof User
来源：http://tbc.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://qzp.epnwcf.com

Ruby: u.is_a?(User)
来源：http://dte.xuetiantiany.cn

C#:   u is User
来源：http://ykn.gogol.net.cn

[G14] 数据类 / record
来源：http://cmf.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://api.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://rid.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://poh.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://gnv.yvedp.cn

Java: record User(String name, int age) {}
来源：http://iyw.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://lvx.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ypb.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://ssx.zhengqikj.top

[G15] 枚举
来源：http://ewn.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hiz.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gpm.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kuv.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rni.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://kzi.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hkz.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://wzr.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gwr.ivvv.top

[G16] 对象转数组 / 字典
来源：http://rxl.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hax.yj202588.top

PHP:  get_object_vars($obj);
来源：http://ahg.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://yue.aibaodan.cn

TS:   Object.entries(obj)
来源：http://cqt.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gcr.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ktu.iojbl.cn

Ruby: obj.instance_variables
来源：http://ksj.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://npr.kuanghao11.cn

================================================================================
来源：http://krq.daria6918.cn

H. 异常与错误处理
来源：http://uea.jqgfzy.top

================================================================================
来源：http://kwc.zycfv.cn

[H01] try / catch 基础
来源：http://osf.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pmt.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oii.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qve.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hnm.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tnf.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gmd.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xhw.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cya.guannengcc.top

[H02] finally / ensure 收尾
来源：http://qmc.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://lag.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ceq.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vfj.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zbr.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gte.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://whq.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wyv.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cac.c1oappe.top

[H03] 主动抛出异常
来源：http://igl.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://exm.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ztu.yongpay.top

JS:   throw new Error("错误信息");
来源：http://csd.yj202588.top

TS:   throw new Error("错误信息");
来源：http://ouk.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ibe.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pic.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kir.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dzb.cucudq.cn

[H04] 自定义异常类型
来源：http://omn.ivvv.top

Py:   class MyError(Exception): pass
来源：http://egj.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gln.aizwys.cn

JS:   class MyError extends Error {}
来源：http://bzz.yvedp.cn

TS:   class MyError extends Error {}
来源：http://cmx.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://tad.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pfu.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://szk.iojbl.cn

C#:   class MyException : Exception {}
来源：http://cfz.uphjek.com

[H05] 捕获特定类型
来源：http://iek.gaohongyu789.top

Py:   except ValueError as e:
来源：http://tca.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cwn.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://jco.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://bas.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://icp.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://erc.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://cwp.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eam.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://qgq.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://avt.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qhe.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qzh.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mlh.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mru.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://agl.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://txz.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://uij.tarul.cn

[H07] 断言
来源：http://yuy.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://uaw.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://wgv.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://zzt.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://vru.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://wjm.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qxc.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zqa.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://whn.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://flt.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://wwk.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://scp.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://zvv.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vmu.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://tid.haohaochexian.top

Go:   err.Error()
来源：http://krg.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://mrj.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://ynj.gogol.net.cn

[H09] 带错误码的异常
来源：http://dko.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cbv.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://klv.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aqm.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gfh.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blk.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oof.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://ntm.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eon.hnqzz.top

[H10] 资源自动释放
来源：http://umf.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jkj.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sxt.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cbm.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ort.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uus.zdqjudy.top

Go:   defer f.Close()
来源：http://axa.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tfw.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qnm.snrcjt.cn

================================================================================
来源：http://dtt.zdqjudy.top

I. 正则表达式
来源：http://rpd.yj20258888.top

================================================================================
来源：http://mwx.yvedp.cn

[I01] 判断是否匹配
来源：http://jnz.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vpx.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vbq.tanke756.top

JS:   /\d+/.test(s)
来源：http://qjg.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://vqr.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mrk.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fqf.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://vxa.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cau.fengsongda.top

[I02] 提取所有匹配
来源：http://dsm.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://ffn.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mpi.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xhm.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://wvd.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lnj.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dtq.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://fvi.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfr.mhx1999.top

[I03] 提取捕获分组
来源：http://nex.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xiq.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qwd.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://omj.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tnp.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dyc.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ntz.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pbz.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://evq.andypj.xyz

[I04] 正则替换
来源：http://exk.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gpt.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cju.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zcs.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://trr.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cdf.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xeg.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ens.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://akz.bbcook.cn

[I05] 按正则拆分
来源：http://ylm.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bqh.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qry.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://axm.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://vwx.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://rfx.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cqm.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://bda.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://paw.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://elq.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uec.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tam.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ggu.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgm.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qnx.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yaa.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pzt.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ccd.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://lxr.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://psp.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kib.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vtb.vqdsnc.cn

TS:   /error/gim
来源：http://bbc.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://exs.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ydo.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://vvs.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nyx.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://hhi.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qog.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxw.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmt.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mpr.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qib.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ydc.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://erw.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vni.fktsv.cn

================================================================================
来源：http://dej.chenlongwang.top

J. 日期与时间
来源：http://agb.shanyushiyangtech.top

================================================================================
来源：http://dzs.tian-w.cn

[J01] 获取当前时间
来源：http://fms.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dnj.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wdp.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://mtf.cheryme.top

TS:   new Date();  Date.now()
来源：http://ljz.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jfi.yueranfly.top

Go:   time.Now()
来源：http://rqo.sweek.top

Ruby: Time.now
来源：http://xze.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dpy.ybcxt.top

[J02] 格式化输出
来源：http://loc.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kzw.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gzx.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dvc.bjfxy.top

TS:   d.toISOString()
来源：http://vel.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rvd.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gyl.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aoq.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lnr.hfpthk.cn

[J03] 字符串解析为日期
来源：http://rlo.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sdc.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dvk.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://oxz.yonumen.top

TS:   new Date("2024-01-02")
来源：http://pma.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://ygq.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cvu.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://lmf.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cjw.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://lfk.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sif.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kvs.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fes.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rhg.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lxp.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qbm.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://buu.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wnd.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://vha.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://vdx.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sjh.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lyw.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jaa.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://gvl.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ukh.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://xhp.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://ozn.ydzc1.top

[J06] 计算两时间之差
来源：http://hya.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://dov.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://eml.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pvx.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://duw.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://qhx.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://xwf.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://yej.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://oxq.hnxiangtu.top

[J07] 比较两个日期
来源：http://sqj.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://gif.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://krq.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://jlo.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://odr.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mex.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdd.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://tur.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://mma.ivvv.top

[J08] 提取年月日与星期
来源：http://dlb.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xda.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gbm.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iwn.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tom.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qxj.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bgs.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tzl.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ijq.zdqjudy.top

[J09] 时区处理
来源：http://qmn.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://erp.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://knu.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gsg.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjg.yangfankeji.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jyl.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://imb.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://apt.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hzj.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://rzv.aibaodan.cn


<!-- 参考信息 -->