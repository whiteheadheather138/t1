代发 wailian999

JS:   get name() { return this._name; }
来源：http://wgn.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://xwz.gogol.net.cn

Java: public String getName() { return name; }
来源：http://fsv.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lkg.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://qzd.meibo888.top

C#:   public string Name { get; set; }
来源：http://bup.meibo888.top

[G12] 对象转字符串
来源：http://ncx.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://oqy.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mwc.yfazqb.com

JS:   toString() { return this.name; }
来源：http://nku.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://vet.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://urp.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://lvt.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://rwe.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://wgs.chenzaomai.com

[G13] 判断对象类型
来源：http://ljb.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://kpv.hnxiangtu.top

PHP:  $u instanceof User
来源：http://rmq.hnqzz.top

JS:   u instanceof User
来源：http://ifo.pengpengdd.cyou

TS:   u instanceof User
来源：http://jao.smart0.xyz

Java: u instanceof User
来源：http://dyv.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://buw.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://liy.shuidangran.top

C#:   u is User
来源：http://myq.xziqi.cn

[G14] 数据类 / record
来源：http://wvy.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xyj.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ezt.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://png.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://zfi.ybcxt.top

Java: record User(String name, int age) {}
来源：http://qvk.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://udy.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uvg.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://bhb.316326.xyz

[G15] 枚举
来源：http://nnk.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xgo.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ohp.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jef.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vfl.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://vdv.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ios.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://hgg.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nor.meibo888.top

[G16] 对象转数组 / 字典
来源：http://rii.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zsf.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://hyz.birdmap.top

JS:   Object.entries(obj)
来源：http://mtp.feifeiyinyue.top

TS:   Object.entries(obj)
来源：http://gwm.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gco.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://obr.cqqwz.cn

Ruby: obj.instance_variables
来源：http://zxc.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://wtg.dianchejie.cn

================================================================================
来源：http://gyi.yongpay.top

H. 异常与错误处理
来源：http://xsc.yj202588.top

================================================================================
来源：http://fmc.tarul.cn

[H01] try / catch 基础
来源：http://feo.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qrj.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pfe.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vsd.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rmr.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://acu.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://elk.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://guq.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ink.tian-w.cn

[H02] finally / ensure 收尾
来源：http://mzg.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://wud.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iwu.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://clq.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lin.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://ayx.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wug.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://bak.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sym.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://xkt.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://hbj.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://shf.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://kuk.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://irp.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://axd.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ice.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ejv.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://eow.daxiang520.top

[H04] 自定义异常类型
来源：http://goj.cashguo.top

Py:   class MyError(Exception): pass
来源：http://uib.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://fln.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://kdb.redwolf501.top

TS:   class MyError extends Error {}
来源：http://wee.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://vag.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://syi.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://pag.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://vuv.zhijiandao.cn

[H05] 捕获特定类型
来源：http://vwg.chenlongwang.top

Py:   except ValueError as e:
来源：http://bhj.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://moa.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://vlt.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://bvt.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://csp.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://alj.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://exm.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vcr.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://jds.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://sbt.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rvv.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://qry.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ovf.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xpz.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cuu.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://yuq.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://oje.yonumen.top

[H07] 断言
来源：http://nbi.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://cod.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://awz.tian-w.cn

JS:   console.assert(x > 0);
来源：http://zrv.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://qrr.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://cck.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mvi.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://jkz.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://wdr.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://wzn.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://wbw.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://epl.zdqjudy.top

JS:   e.message;  e.stack
来源：http://mmf.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lit.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://omi.hnxiangtu.top

Go:   err.Error()
来源：http://tpz.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://xyq.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://dsr.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://egq.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://teq.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vtm.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ssf.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hzm.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vsa.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wwv.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hxp.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ebr.nwbrower.top

[H10] 资源自动释放
来源：http://iuc.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fwu.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kzc.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dpz.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jdb.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://esd.xylfe.cn

Go:   defer f.Close()
来源：http://kjz.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://knn.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wno.jlsjyb.cn

================================================================================
来源：http://pvt.zhiwuduotai.top

I. 正则表达式
来源：http://ycg.tianlin.xyz

================================================================================
来源：http://fmk.0kj1m.cn

[I01] 判断是否匹配
来源：http://pnv.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nsu.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://jmb.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://feq.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://tvy.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fnn.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iwx.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://czh.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yej.guannengcc.top

[I02] 提取所有匹配
来源：http://vho.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://rnz.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nii.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://knf.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://rzf.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kmo.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://goa.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://shd.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qqv.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://kms.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ins.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cow.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cjv.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fne.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ldj.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sqf.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://boo.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://isi.xylfe.cn

[I04] 正则替换
来源：http://uxq.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vqo.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wni.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ywm.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://iny.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://dwp.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ist.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yvw.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bqh.zdqjudy.top

[I05] 按正则拆分
来源：http://ixf.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vhm.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jop.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://euo.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://xcs.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://qul.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lnj.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://zer.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgq.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wno.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hnu.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ihq.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fva.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aqk.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tbc.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hjx.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tbs.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vvg.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://rzf.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ato.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fuw.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wuq.sxryk.cn

TS:   /error/gim
来源：http://lzh.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lsv.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://npd.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://lkh.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://has.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://ijq.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dsc.guowangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dhy.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jwm.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tzp.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vrq.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://unr.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ncc.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ums.fanxiaobao.xyz

================================================================================
来源：http://qux.sxryk.cn

J. 日期与时间
来源：http://hva.fehbvm.com

================================================================================
来源：http://wae.9152youxi.cn

[J01] 获取当前时间
来源：http://bya.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xle.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cjz.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://vao.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://fuj.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ogt.ywan-chungtsiang.top

Go:   time.Now()
来源：http://qmf.nanxuanxn.top

Ruby: Time.now
来源：http://gsq.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ewo.jinqigufen.top

[J02] 格式化输出
来源：http://ngh.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frs.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uvw.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iwp.yanxiufei.cn

TS:   d.toISOString()
来源：http://jqp.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://amw.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jmy.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oxl.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://obp.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://xkl.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iwe.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jmv.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://nzm.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://akf.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://cqb.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://agh.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://axj.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vyc.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://yti.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uqx.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eji.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tbe.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sqq.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://obp.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iki.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bzf.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zpd.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://vil.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://hqa.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xqn.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://med.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kmc.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://arv.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://olg.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://vaw.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://qhg.pycfn.com

[J06] 计算两时间之差
来源：http://eyd.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://tdw.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://vft.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://twg.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://txz.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://her.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://jzv.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://ape.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://dhi.ehwqpu.com

[J07] 比较两个日期
来源：http://fbz.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://bzu.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wxi.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kwe.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mmm.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jhf.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://izj.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://hsu.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://zem.zdbjq.cn

[J08] 提取年月日与星期
来源：http://vxr.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lez.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lxo.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uly.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ccc.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xea.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://byz.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ind.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jwb.smart0.xyz

[J09] 时区处理
来源：http://wjr.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://twc.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nty.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tij.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wyg.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kvs.yangfankeji.com


<!-- 参考信息 -->