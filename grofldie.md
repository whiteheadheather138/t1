代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://rnn.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://oyq.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://adi.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://egr.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gif.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://sml.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://qek.jlsjyb.cn

[G13] 判断对象类型
来源：http://gfn.yj20258.top

Py:   isinstance(u, User)
来源：http://uug.316326.xyz

PHP:  $u instanceof User
来源：http://myi.zdqjudy.top

JS:   u instanceof User
来源：http://yow.hesvh.cn

TS:   u instanceof User
来源：http://ikb.fehbvm.com

Java: u instanceof User
来源：http://msh.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gdf.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://xvq.zhaomingkeji.xyz

C#:   u is User
来源：http://dcz.uphjek.com

[G14] 数据类 / record
来源：http://gxe.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wzm.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://ufp.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://gdq.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://tbr.sysykeji.top

Java: record User(String name, int age) {}
来源：http://mff.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://uoy.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gst.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://lkr.gzhubu.top

[G15] 枚举
来源：http://rel.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ovg.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pgk.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xzs.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hnc.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://qta.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jnu.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://alz.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zmo.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://skh.sxryk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cqu.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://pjo.meibo888.top

JS:   Object.entries(obj)
来源：http://dzk.ppjwa.cn

TS:   Object.entries(obj)
来源：http://esy.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://keh.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://nzd.gogol.net.cn

Ruby: obj.instance_variables
来源：http://cbg.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://qnu.gzhubu.top

================================================================================
来源：http://bzq.yonumen.top

H. 异常与错误处理
来源：http://zsn.chenjidiqi.icu

================================================================================
来源：http://cfj.chenzaomai.com

[H01] try / catch 基础
来源：http://vch.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rws.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ztd.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://brp.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ldu.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ljn.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gpp.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fmn.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zwx.andypj.xyz

[H02] finally / ensure 收尾
来源：http://kuz.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://nwo.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ees.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://avt.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://smn.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://fzz.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://efv.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ido.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://tao.316326.xyz

[H03] 主动抛出异常
来源：http://jpf.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://lma.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lzz.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://wim.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://pct.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iol.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jis.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://thp.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://ugk.yonumen.top

[H04] 自定义异常类型
来源：http://cmb.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://juh.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://rne.52xcode.cn

JS:   class MyError extends Error {}
来源：http://als.xylfe.cn

TS:   class MyError extends Error {}
来源：http://waj.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://yak.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pyr.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://wee.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://ple.hnqzz.top

[H05] 捕获特定类型
来源：http://gat.hfpthk.cn

Py:   except ValueError as e:
来源：http://vcp.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lmk.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://wib.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://zqd.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://wbt.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xlu.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://pzm.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://edu.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://ula.havefunace.top

Py:   value = d.get("k") or default
来源：http://uru.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://bfu.nwbrower.top

JS:   obj?.a?.b;  d ?? default
来源：http://wwl.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://baf.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xus.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uuq.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://qdk.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://guk.ybcxt.top

[H07] 断言
来源：http://oma.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://mbd.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://fgk.yongpay.top

JS:   console.assert(x > 0);
来源：http://btm.ivvv.top

TS:   console.assert(x > 0);
来源：http://hab.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://wub.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ant.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://drg.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://gfb.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://jvy.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://cty.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://djw.bjfxy.top

JS:   e.message;  e.stack
来源：http://tru.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zil.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kgt.hnqzz.top

Go:   err.Error()
来源：http://fdu.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://mbi.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://aud.nanxuanxn.top

[H09] 带错误码的异常
来源：http://kxz.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aak.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cnz.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kij.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yqu.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bek.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lxc.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://ovy.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mrp.yueranfly.top

[H10] 资源自动释放
来源：http://dsw.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jga.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sku.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nkg.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eda.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pnz.0kj1m.cn

Go:   defer f.Close()
来源：http://waf.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zoy.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://szi.jiagoushi.top

================================================================================
来源：http://wcx.tarul.cn

I. 正则表达式
来源：http://spy.zdqjudy.top

================================================================================
来源：http://vqf.sysykeji.top

[I01] 判断是否匹配
来源：http://qhp.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lbp.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hca.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://ous.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://ssb.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vbr.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ota.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://xrg.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nyd.meibo888.top

[I02] 提取所有匹配
来源：http://gqo.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://sib.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dzp.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fjv.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://vpk.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jaj.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xzz.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://dui.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zvk.daxiang520.top

[I03] 提取捕获分组
来源：http://ayx.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bes.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://knc.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://anh.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qvx.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xpv.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vfn.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ntk.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://thw.shzxlz.cn

[I04] 正则替换
来源：http://nse.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hsp.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jqd.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jpb.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://arw.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ikm.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://umm.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tsn.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fnb.cqqwz.cn

[I05] 按正则拆分
来源：http://wic.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pje.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://raj.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://fgw.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://qlc.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://cdc.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yws.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://hin.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ner.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oss.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zwf.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://otb.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vun.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqn.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qwz.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pnz.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wtn.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsg.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://axv.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oqa.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hwa.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bkf.svipenyu.cn

TS:   /error/gim
来源：http://bah.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rrp.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hbp.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://fcx.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hli.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://xpw.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://utx.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://veo.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ugu.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mjc.guannengcc.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ksw.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bon.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://idn.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wqr.chenlongwang.top

================================================================================
来源：http://kwc.havefunace.top

J. 日期与时间
来源：http://lrx.wangshuangyany.cn

================================================================================
来源：http://hpr.dashuyun.cn

[J01] 获取当前时间
来源：http://rpg.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://plv.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://avi.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://awf.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://fgk.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kyy.sufxvd.cn

Go:   time.Now()
来源：http://fxm.yangfankeji.com

Ruby: Time.now
来源：http://ger.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ykm.shzxlz.cn

[J02] 格式化输出
来源：http://znx.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uch.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zfd.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hxy.yj20258888.top

TS:   d.toISOString()
来源：http://tkx.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xck.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ynt.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqm.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fez.cucudq.cn

[J03] 字符串解析为日期
来源：http://bjx.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wdb.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fup.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://osg.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://jmv.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://emt.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tnu.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://hez.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qnt.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://xbt.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vcm.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wth.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://leb.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://miu.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://izx.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cmf.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://epl.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qvr.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://esu.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://uhm.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ynk.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://air.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ako.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://uwh.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://avf.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://gyf.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://njv.hysaishi.cn

[J06] 计算两时间之差
来源：http://zwp.tanke756.top

Py:   (end - start).total_seconds()
来源：http://ygw.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://jzf.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rsl.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://stg.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://wad.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://zku.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://urc.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://bba.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://zkm.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://wcm.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pmy.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://phr.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://isg.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cyv.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qwu.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://kss.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://nfj.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://uof.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gfe.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uzj.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://arj.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wwl.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qay.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mol.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbr.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wwo.316326.xyz

[J09] 时区处理
来源：http://aju.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pkm.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vee.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tda.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kjd.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mot.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kqd.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://szu.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xlr.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://lzz.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://azl.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zio.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sxw.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kbo.sysykeji.top


<!-- 参考信息 -->