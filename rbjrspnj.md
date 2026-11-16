代发 wailian999

[G10] 访问控制
来源：http://zni.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://fpj.hammf.cn

PHP:  public / protected / private
来源：http://cyd.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://wau.haohaochexian.top

TS:   public / protected / private
来源：http://wkc.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://etf.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gva.guowangkeji.top

Ruby: public / protected / private
来源：http://aqk.zycfv.cn

C#:   public / protected / private / internal
来源：http://ztt.jiagoushi.top

[G11] getter / setter
来源：http://aeg.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://wnz.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wto.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://pce.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://hqo.tarul.cn

Java: public String getName() { return name; }
来源：http://rjq.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hgc.hammf.cn

Ruby: attr_accessor :name
来源：http://bre.smart0.xyz

C#:   public string Name { get; set; }
来源：http://fut.ybcxt.top

[G12] 对象转字符串
来源：http://hzn.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://czo.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gmf.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://bof.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://orm.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://ahi.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://euv.hcnkem.com

Ruby: def to_s; @name; end
来源：http://rnr.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://jwv.havefunace.top

[G13] 判断对象类型
来源：http://uub.guowangkeji.top

Py:   isinstance(u, User)
来源：http://jel.vehdjk.com

PHP:  $u instanceof User
来源：http://kay.sweek.top

JS:   u instanceof User
来源：http://hsn.jyoumei.cn

TS:   u instanceof User
来源：http://aln.yuanzhike.top

Java: u instanceof User
来源：http://ghu.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://swv.xuanzx.com

Ruby: u.is_a?(User)
来源：http://cnx.shangyingyoupin.top

C#:   u is User
来源：http://zch.hammf.cn

[G14] 数据类 / record
来源：http://joh.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hyj.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://tnk.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ubj.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://nqj.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://bfq.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://bhm.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kcf.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://qpx.birdmap.top

[G15] 枚举
来源：http://bms.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jxb.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zij.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jqr.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bow.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://vii.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fof.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://juo.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qws.hammf.cn

[G16] 对象转数组 / 字典
来源：http://sjb.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fxq.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://egg.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://wwm.gzhubu.top

TS:   Object.entries(obj)
来源：http://soc.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dik.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hvm.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://vwb.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://qvh.sysykeji.top

================================================================================
来源：http://mbv.ybcxt.top

H. 异常与错误处理
来源：http://gik.hesvh.cn

================================================================================
来源：http://wgx.gogol.net.cn

[H01] try / catch 基础
来源：http://zhq.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://roj.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ajl.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://our.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kwx.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fye.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pje.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pkn.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rtb.nanxinkj.top

[H02] finally / ensure 收尾
来源：http://qqm.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dyc.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fzr.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hjr.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xtt.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://ara.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fbx.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://eur.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lcy.sjlbkw.cn

[H03] 主动抛出异常
来源：http://ljg.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://czx.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rou.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://ayk.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://tvl.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qwz.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ush.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nch.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qxl.redwolf501.top

[H04] 自定义异常类型
来源：http://gbx.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://tuk.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vjh.shuidangran.top

JS:   class MyError extends Error {}
来源：http://dqf.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://wbh.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://mos.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sbu.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://lkr.sxryk.cn

C#:   class MyException : Exception {}
来源：http://nmk.chenlongwang.top

[H05] 捕获特定类型
来源：http://uwd.zhixingplan.top

Py:   except ValueError as e:
来源：http://wmy.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vey.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://eie.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://gkx.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://gvx.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cmk.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://nww.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ebm.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://eyl.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://mzy.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://tnh.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://ezz.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://vnm.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uqz.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rnm.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://yyl.sweek.top

C#:   obj?.A?.B ?? default
来源：http://lra.birdmap.top

[H07] 断言
来源：http://pmw.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://cwt.yfazqb.com

PHP:  assert($x > 0);
来源：http://iic.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://zvr.tarul.cn

TS:   console.assert(x > 0);
来源：http://afd.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://olp.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgq.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://kam.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://vtf.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://wfq.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://uni.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dxa.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://hpe.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://mzq.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kjz.sjlbkw.cn

Go:   err.Error()
来源：http://kod.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://mmy.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://fzn.zhixingplan.top

[H09] 带错误码的异常
来源：http://ngp.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bzv.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ouu.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iis.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://edp.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dif.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://byl.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xet.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mkk.mhx1999.top

[H10] 资源自动释放
来源：http://ywi.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bdk.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ygq.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dem.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bxw.ywan-chungtsiang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ila.yj20258.top

Go:   defer f.Close()
来源：http://kqa.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dpe.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lfc.uphjek.com

================================================================================
来源：http://hvh.redwolf501.top

I. 正则表达式
来源：http://the.iojbl.cn

================================================================================
来源：http://vgs.wangdashe.top

[I01] 判断是否匹配
来源：http://xha.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lnk.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://fva.cheryme.top

JS:   /\d+/.test(s)
来源：http://zms.tian-w.cn

TS:   /\d+/.test(s)
来源：http://scz.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gvy.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tmo.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://lrb.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ale.jianghu66.top

[I02] 提取所有匹配
来源：http://dzk.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://vuu.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ira.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yda.meibo888.top

TS:   s.match(/\d+/g)
来源：http://nje.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://erg.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ppt.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://rgn.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rkj.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://isl.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cet.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://csf.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://coo.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fug.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vaf.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aaj.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qzq.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://acw.yvedp.cn

[I04] 正则替换
来源：http://cna.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vsm.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nju.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ojt.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://bgm.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dqt.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yow.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dqa.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://htd.hfpthk.cn

[I05] 按正则拆分
来源：http://vez.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ksq.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mmm.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://wre.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://hzu.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://qzw.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fro.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://art.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vcz.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bqq.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://trn.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wij.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wtr.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twv.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fmi.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://svo.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mho.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qsn.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://lqa.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vys.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lqk.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tlu.chenjidiqi.icu

TS:   /error/gim
来源：http://jxd.nanxinkj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hmv.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yaj.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://zoc.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mez.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://mky.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qcq.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qhv.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgz.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dly.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bnh.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mlk.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xwl.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cwo.zhaomingkeji.xyz

================================================================================
来源：http://wkg.zhaomingkeji.xyz

J. 日期与时间
来源：http://bka.tanke756.top

================================================================================
来源：http://kia.sweek.top

[J01] 获取当前时间
来源：http://yum.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://kmj.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rxu.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://xqc.hammf.cn

TS:   new Date();  Date.now()
来源：http://yfi.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://det.c1oappe.top

Go:   time.Now()
来源：http://kqb.hammf.cn

Ruby: Time.now
来源：http://zms.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://exi.daxiang520.top

[J02] 格式化输出
来源：http://bwj.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ecx.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kiv.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ohi.jyoumei.cn

TS:   d.toISOString()
来源：http://edp.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rtn.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://udn.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bse.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xtl.jyoumei.cn

[J03] 字符串解析为日期
来源：http://lkr.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kll.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xvi.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://wmv.tanke756.top

TS:   new Date("2024-01-02")
来源：http://gwf.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://hio.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vzc.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://lni.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pko.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://xrf.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fqc.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xel.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://guj.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eyl.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gfg.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kuy.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ipo.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vie.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://mwm.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://zbi.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ofu.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tgf.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhu.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://rtl.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tvo.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://uzu.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://jkl.fehbvm.com

[J06] 计算两时间之差
来源：http://ldi.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://oed.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://ekh.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cke.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baf.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vgv.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://sjh.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://gow.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://ulh.bjfxy.top

[J07] 比较两个日期
来源：http://ucx.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://sbz.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iwb.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fkm.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tcz.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://imi.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pgo.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://wci.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://kja.ehwqpu.com

[J08] 提取年月日与星期
来源：http://dnf.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://evz.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://izu.yuanzhike.top


<!-- 参考信息 -->