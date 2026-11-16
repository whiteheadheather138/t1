代发 wailian999

JS:   get name() { return this._name; }
来源：http://rom.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://pfa.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://kzq.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://uly.cucudq.cn

Ruby: attr_accessor :name
来源：http://gpx.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://nct.quarkkingdee.top

[G12] 对象转字符串
来源：http://hed.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://ynk.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://reo.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://cxz.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://fdx.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://rof.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://lmb.yfazqb.com

Ruby: def to_s; @name; end
来源：http://irv.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://bli.hfpthk.cn

[G13] 判断对象类型
来源：http://nvt.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://jyp.zhengqikj.top

PHP:  $u instanceof User
来源：http://bjw.yj20258888.top

JS:   u instanceof User
来源：http://agf.jinghuilouyu.cn

TS:   u instanceof User
来源：http://viq.jiagoushi.top

Java: u instanceof User
来源：http://qqd.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ato.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://lyx.9152youxi.cn

C#:   u is User
来源：http://chq.yanxiufei.cn

[G14] 数据类 / record
来源：http://ooh.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bjm.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://wkk.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://srg.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://zaj.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://pkq.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://fmd.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pmw.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://hhm.0kj1m.cn

[G15] 枚举
来源：http://lrj.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ajr.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://fom.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xbu.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lbo.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://zos.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qbk.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://zsb.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wjs.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://uwo.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jzz.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://ddi.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://qrr.zdbjq.cn

TS:   Object.entries(obj)
来源：http://rhq.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uxi.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wxk.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://gfu.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://loy.quarkkingdee.top

================================================================================
来源：http://jvu.shangyingyoupin.top

H. 异常与错误处理
来源：http://qnp.ywan-chungtsiang.top

================================================================================
来源：http://ell.andypj.xyz

[H01] try / catch 基础
来源：http://yul.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ekx.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yws.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://znh.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ugh.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ymf.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fds.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qgs.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zbx.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://pif.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://nwp.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mnr.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://onx.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wpo.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://kgh.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wff.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://deb.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fun.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://elg.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://hwh.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vef.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://uvs.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://ifh.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bgi.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ovx.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cfm.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://rnn.dianchejie.cn

[H04] 自定义异常类型
来源：http://srw.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://hsv.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://mvc.iojbl.cn

JS:   class MyError extends Error {}
来源：http://cap.yj20258888.top

TS:   class MyError extends Error {}
来源：http://rug.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://dku.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cww.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://zzi.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://ubx.jlsjyb.cn

[H05] 捕获特定类型
来源：http://olv.shuidangran.top

Py:   except ValueError as e:
来源：http://mhw.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://psl.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://ifw.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://tbm.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://pjt.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://omv.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://rvj.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zig.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://uhc.cashguo.top

Py:   value = d.get("k") or default
来源：http://ydc.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://gpc.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://ole.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://rtk.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rkg.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://msc.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://hhu.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://ujd.iojbl.cn

[H07] 断言
来源：http://ywk.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://zoo.yangfankeji.com

PHP:  assert($x > 0);
来源：http://xto.xziqi.cn

JS:   console.assert(x > 0);
来源：http://fdb.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://bfy.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ewb.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://por.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cuq.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://hbu.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://mwt.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://nox.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yll.fehbvm.com

JS:   e.message;  e.stack
来源：http://mit.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://osh.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xyo.c1oappe.top

Go:   err.Error()
来源：http://alk.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://jig.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://obn.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://dud.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jfs.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://gnc.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ddd.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cvb.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qhd.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gce.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://njo.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://txs.nanxuanxn.top

[H10] 资源自动释放
来源：http://tbe.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xhb.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ods.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ixd.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hru.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jhi.sxryk.cn

Go:   defer f.Close()
来源：http://ymi.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gxy.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vqv.chenzaomai.com

================================================================================
来源：http://aac.jinqigufen.top

I. 正则表达式
来源：http://fkw.fktsv.cn

================================================================================
来源：http://gdi.guowangkeji.top

[I01] 判断是否匹配
来源：http://qlv.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hod.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jah.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://qcy.wangdashe.top

TS:   /\d+/.test(s)
来源：http://epm.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nwn.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kon.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://bqw.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pjh.andypj.xyz

[I02] 提取所有匹配
来源：http://zgv.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://xiy.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xaq.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ntl.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://wjd.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mfv.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wxy.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://llx.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rcu.nanxuanxn.top

[I03] 提取捕获分组
来源：http://fqo.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbd.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wpa.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfq.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qub.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xcn.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bze.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cut.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rhj.quarkkingdee.top

[I04] 正则替换
来源：http://ebx.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oxu.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vmc.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://iuk.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ild.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://ham.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wly.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://elb.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vny.0kj1m.cn

[I05] 按正则拆分
来源：http://xin.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kdm.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wla.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://umb.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://kwd.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://fob.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ari.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://mko.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cvq.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://emb.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ajh.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dtc.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cav.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksx.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lzs.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cby.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fft.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nrs.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://szi.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eqn.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pmc.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://amr.gotoacloud.top

TS:   /error/gim
来源：http://mxf.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://chn.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oys.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://xnj.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jdl.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://qby.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xht.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://imh.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvg.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yib.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ywt.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://swc.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mrz.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iqc.yj202588.top

================================================================================
来源：http://ivm.yj20258.top

J. 日期与时间
来源：http://nip.dianchejie.cn

================================================================================
来源：http://ovc.uphjek.com

[J01] 获取当前时间
来源：http://ety.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vuw.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mzi.andypj.xyz

JS:   new Date();  Date.now()
来源：http://idn.mhx1999.top

TS:   new Date();  Date.now()
来源：http://qsq.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://deo.zdqjudy.top

Go:   time.Now()
来源：http://kpa.hnqzz.top

Ruby: Time.now
来源：http://xjk.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bik.vqdsnc.cn

[J02] 格式化输出
来源：http://jjz.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wea.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cac.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kgd.nanxinkj.top

TS:   d.toISOString()
来源：http://his.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://okt.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dtl.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kel.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hox.svipenyu.cn

[J03] 字符串解析为日期
来源：http://dun.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zen.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dra.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://iez.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://cfd.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://cyn.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://btc.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lrh.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dsz.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://pvi.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xwm.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fiu.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xmt.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ogr.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pfp.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zmd.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rlb.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ypq.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://tgv.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://sly.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ugc.c1oappe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmt.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dxw.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://dwm.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zkq.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://dah.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iwk.ybcxt.top

[J06] 计算两时间之差
来源：http://cyp.tarul.cn

Py:   (end - start).total_seconds()
来源：http://urs.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://ibf.316326.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://syn.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rid.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://aws.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://moq.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://cbl.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://and.zycfv.cn

[J07] 比较两个日期
来源：http://iku.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://yha.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mvg.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://bfy.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ups.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://znd.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qic.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://eyr.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://xna.daria6918.cn

[J08] 提取年月日与星期
来源：http://fnp.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jzp.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wcd.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vzz.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qmz.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vur.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qmr.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gmf.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pbw.gaohongyu789.top

[J09] 时区处理
来源：http://vhj.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hrr.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ydj.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avc.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzi.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pat.jyoumei.cn


<!-- 参考信息 -->