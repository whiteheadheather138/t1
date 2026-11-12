代发 wailian999

C#:   public / protected / private / internal
来源：http://ypo.jqgfzy.top

[G11] getter / setter
来源：http://ynj.yonumen.top

Py:   @property 与 @x.setter
来源：http://zxr.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hnx.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://yuj.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://bfi.sxryk.cn

Java: public String getName() { return name; }
来源：http://yaz.jqgfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tid.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://fid.iojbl.cn

C#:   public string Name { get; set; }
来源：http://sbs.yj20258.top

[G12] 对象转字符串
来源：http://sft.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://nrz.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fdv.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://jyx.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://brm.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://sjp.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://hma.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://lfa.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://wjo.zhiwuduotai.top

[G13] 判断对象类型
来源：http://say.yj20258888.top

Py:   isinstance(u, User)
来源：http://zgt.havefunace.top

PHP:  $u instanceof User
来源：http://nnh.jlsjyb.cn

JS:   u instanceof User
来源：http://svm.cheryme.top

TS:   u instanceof User
来源：http://lbx.uphjek.com

Java: u instanceof User
来源：http://egr.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ude.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://muj.yj202588.top

C#:   u is User
来源：http://thf.vqdsnc.cn

[G14] 数据类 / record
来源：http://zhs.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fcs.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://abk.jiagoushi.top

JS:   // 无内置：普通类或对象字面量
来源：http://ztw.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://yyg.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://ywc.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://iuh.hfpthk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://otf.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://mcf.gaohongyu789.top

[G15] 枚举
来源：http://hcs.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ifb.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bkm.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mwz.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ptg.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://kjv.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cni.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://nsb.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bdq.uphjek.com

[G16] 对象转数组 / 字典
来源：http://szd.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bcn.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://dvz.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://jae.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://hxk.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lyg.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://goq.yvedp.cn

Ruby: obj.instance_variables
来源：http://kmn.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://exw.zhijiandao.cn

================================================================================
来源：http://mcj.yangfankeji.com

H. 异常与错误处理
来源：http://ixk.ppjwa.cn

================================================================================
来源：http://qpi.ppjwa.cn

[H01] try / catch 基础
来源：http://etd.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://umu.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xqz.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rho.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fqj.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ciq.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ycd.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uwz.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kes.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://psu.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tba.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qsg.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bvx.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lkw.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://abe.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fej.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://szy.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ndv.snrcjt.cn

[H03] 主动抛出异常
来源：http://wzd.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://msw.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xup.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://sbp.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://ufv.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zpu.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tjk.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://igh.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://dao.sysykeji.top

[H04] 自定义异常类型
来源：http://nem.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://lxp.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mod.tarul.cn

JS:   class MyError extends Error {}
来源：http://pzf.ydzc1.top

TS:   class MyError extends Error {}
来源：http://kwd.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://tta.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qco.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://ipq.meibo888.top

C#:   class MyException : Exception {}
来源：http://lgu.nanxinkj.top

[H05] 捕获特定类型
来源：http://vae.hfpthk.cn

Py:   except ValueError as e:
来源：http://bhw.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sir.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://plo.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://nei.shanyushiyangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://bkl.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://elg.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://qtl.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://enj.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://avp.daria6918.cn

Py:   value = d.get("k") or default
来源：http://xvq.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xtv.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://ycl.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wuf.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://flx.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gdr.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://yfl.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://qcj.jqgfzy.top

[H07] 断言
来源：http://nnf.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://dfl.yj20258888.top

PHP:  assert($x > 0);
来源：http://mwa.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://yqe.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://xik.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://lgc.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vis.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://unv.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://uqi.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://hwn.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://yaa.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qef.gzhubu.top

JS:   e.message;  e.stack
来源：http://uwd.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dem.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://msh.zhongyouzk.top

Go:   err.Error()
来源：http://mtg.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://nto.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://vxs.tanke756.top

[H09] 带错误码的异常
来源：http://ewf.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dyc.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ssb.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fbl.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zgf.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fzm.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kqh.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://sew.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zoq.fzhhl.top

[H10] 资源自动释放
来源：http://ytt.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rmv.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sdr.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dtl.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://opm.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pmf.yvedp.cn

Go:   defer f.Close()
来源：http://ema.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qjt.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uuu.daxiang520.top

================================================================================
来源：http://ksg.tianlin.xyz

I. 正则表达式
来源：http://qav.gzhubu.top

================================================================================
来源：http://cdu.guowangkeji.top

[I01] 判断是否匹配
来源：http://gzl.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xnl.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wdk.fzhhl.top

JS:   /\d+/.test(s)
来源：http://ckd.uphjek.com

TS:   /\d+/.test(s)
来源：http://iie.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gkc.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cdy.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://zfh.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://udb.yonumen.top

[I02] 提取所有匹配
来源：http://gpe.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://whq.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://waz.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ryx.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://iit.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hrb.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ynw.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://yxm.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vfk.hysaishi.cn

[I03] 提取捕获分组
来源：http://zzf.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dih.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pbx.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xfy.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gag.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jxx.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tkq.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wiz.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mfv.ehwqpu.com

[I04] 正则替换
来源：http://ruu.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cme.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bgs.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://hvr.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://lmw.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://iwf.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://voc.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://mqz.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ebn.xinyue.icu

[I05] 按正则拆分
来源：http://xwb.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://azt.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cxq.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://bpw.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://wqc.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://vjx.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iav.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://fzg.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hye.meibo888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oud.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdi.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zxb.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldp.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zzn.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://htu.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cxr.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fdb.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bdr.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://zim.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nwz.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fbm.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xmz.vehdjk.com

TS:   /error/gim
来源：http://yky.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nld.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://knk.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://hdg.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://diy.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://wka.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ccp.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsk.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vua.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://izw.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rfq.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zjt.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://doo.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nlg.hnqzz.top

================================================================================
来源：http://raf.bbcook.cn

J. 日期与时间
来源：http://div.zhoulong.xyz

================================================================================
来源：http://jij.jinqigufen.top

[J01] 获取当前时间
来源：http://trf.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dhk.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fzm.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://ftc.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://brx.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kud.jinqigufen.top

Go:   time.Now()
来源：http://olq.birdmap.top

Ruby: Time.now
来源：http://law.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://efe.chenlongwang.top

[J02] 格式化输出
来源：http://bav.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ygy.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ntv.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nfc.vehdjk.com

TS:   d.toISOString()
来源：http://cdu.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwn.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nfm.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fjw.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kgp.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://tzf.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sjx.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlt.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://wjd.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://fir.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://zus.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ysz.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://rli.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cfi.yfazqb.com

[J04] 时间戳与日期互转
来源：http://ryo.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ivf.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qcg.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hwv.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zrp.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fhu.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qiy.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uvy.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fvz.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://owq.sweek.top

Py:   now + timedelta(days=7)
来源：http://iid.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sos.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://owy.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cqt.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://pjf.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://unq.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://nuh.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://rva.bbcook.cn

[J06] 计算两时间之差
来源：http://yst.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://nyg.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://dam.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://joa.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jlb.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fyo.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://ine.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://hhu.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://seu.zycfv.cn

[J07] 比较两个日期
来源：http://ibn.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://api.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://laa.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://uqx.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://vor.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fun.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qhy.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://tgt.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gzw.yj20258.top

[J08] 提取年月日与星期
来源：http://abe.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fsp.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iiu.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jby.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fra.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://reo.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ulq.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vve.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pmi.fengsongda.top

[J09] 时区处理
来源：http://bja.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jml.guannengcc.top


<!-- 参考信息 -->