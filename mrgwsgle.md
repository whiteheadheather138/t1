代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xcq.shzxlz.cn

[Q75] 日期格式化
来源：http://ynq.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hsv.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sjs.cqqwz.cn

[Q76] 按天统计
来源：http://cpe.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gsw.nwbrower.top

[Q77] 时间加减
来源：http://pap.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://usm.hysaishi.cn

[Q78] 当前时间
来源：http://crj.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wor.fengsongda.top

[Q79] 字符串拼接
来源：http://led.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://loc.hammf.cn

[Q80] 字符串截取
来源：http://aqa.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jac.yongpay.top

[Q81] 字符串替换
来源：http://zui.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jqs.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://tbo.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bxn.yvedp.cn

[Q83] 大小写转换
来源：http://dmm.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kgf.tarul.cn

[Q84] 去除首尾空格
来源：http://fli.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://voh.52xcode.cn

[Q85] 数值取整
来源：http://jgm.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oxr.uphjek.com

[Q86] 读取 JSON 字段
来源：http://btz.yj202588.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cxr.nanxuanxn.top

[Q87] JSON 字段做条件
来源：http://eiv.xuanzx.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lzh.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://gra.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wfx.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mon.iojbl.cn

[Q89] 判断表是否存在
来源：http://dqs.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://muq.redwolf501.top

[Q90] 生成序号列
来源：http://buo.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kwz.zhengqikj.top

================================================================================
来源：http://kqu.sufxvd.cn

R. Bash 专题
来源：http://ybs.yanxiufei.cn

================================================================================
来源：http://ivh.zdbjq.cn

[R01] shebang 与严格模式
来源：http://lps.0kj1m.cn

#!/usr/bin/env bash
来源：http://wjw.yanxiufei.cn

set -euo pipefail
来源：http://lyo.mhx1999.top

[R02] 变量赋值与使用
来源：http://yet.yuxming.cn

name="Tom"; echo "$name"
来源：http://dxl.yangfankeji.com

[R03] 只读变量
来源：http://tcj.hysaishi.cn

readonly PI=3.14
来源：http://akm.jlsjyb.cn

[R04] 位置参数
来源：http://onh.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zut.dianchejie.cn

[R05] 参数默认值
来源：http://gfd.cdnleiting.top

name="${1:-default}"
来源：http://ugs.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://aau.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hjk.xuanzx.com

[R07] if 判断文件
来源：http://ilg.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ifj.iojbl.cn

[R08] 数值比较
来源：http://imr.quarkkingdee.top

if (( a > b )); then echo "a 更大"; fi
来源：http://noa.zhijiandao.cn

[R09] 字符串比较
来源：http://plw.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pcp.ydjk.org.cn

[R10] 正则匹配
来源：http://jmi.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kad.hongshengwenyu.top

[R11] case 多分支
来源：http://rfy.sysykeji.top

case "$1" in
来源：http://kxy.shuidangran.top

start) echo "启动" ;;
来源：http://xlk.yj202588.top

stop)  echo "停止" ;;
来源：http://tdu.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://mla.gogol.net.cn

esac
来源：http://tjg.yj20258.top

[R12] for 遍历文件
来源：http://qgl.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://cdl.zdbjq.cn

[R13] for 计数循环
来源：http://bci.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://rzr.yuanzhike.top

[R14] C 风格 for
来源：http://iqt.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hxe.316326.xyz

[R15] while 逐行读文件
来源：http://fjm.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uxx.tarul.cn

[R16] until 等待条件
来源：http://ros.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ugu.aibaodan.cn

[R17] 数组定义与取值
来源：http://eps.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://gba.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://spe.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hhk.jyoumei.cn

[R19] 数组长度
来源：http://yfz.jlsjyb.cn

echo "${#arr[@]}"
来源：http://kfe.sysykeji.top

[R20] 关联数组（字典）
来源：http://uyt.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nsu.aizwys.cn

[R21] 字符串长度
来源：http://zoc.cqqwz.cn

echo "${#s}"
来源：http://rbw.shanyushiyangtech.top

[R22] 截取子串
来源：http://ydt.xinyue.icu

echo "${s:0:5}"
来源：http://ish.sweek.top

[R23] 字符串替换
来源：http://kvq.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vzy.xylfe.cn

[R24] 大小写转换
来源：http://ygg.zhaomingkeji.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://mir.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://tsb.wangshuangyany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://meu.ydzc1.top

[R26] 命令替换
来源：http://rno.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://jrz.9152youxi.cn

[R27] 算术展开
来源：http://srj.epnwcf.com

echo $((1 + 2 * 3))
来源：http://ujl.zycfv.cn

[R28] 浮点运算
来源：http://sgx.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://zdm.daxiang520.top

[R29] 定义函数
来源：http://imf.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xrd.sjlbkw.cn

[R30] 函数返回状态码
来源：http://zzl.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://qzg.smart0.xyz

[R31] 局部变量
来源：http://lia.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://ysm.gaohongyu789.top

[R32] 参数个数校验
来源：http://tpv.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aoz.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://pfm.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jpw.tanke756.top

[R34] 退出时清理
来源：http://eou.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://vhi.jinqigfzy.top

[R35] 后台执行并等待
来源：http://oyz.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tnq.ehwqpu.com

[R36] 并发执行多个任务
来源：http://sfd.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cfj.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://rxq.fengsongda.top

files=$(ls -1)
来源：http://zkk.vqdsnc.cn

[R38] 管道串联
来源：http://yyf.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://loj.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://udt.xinyue.icu

cmd > out.log 2>&1
来源：http://uka.ydzc1.top

[R40] 追加写日志
来源：http://rct.zhengqikj.top

echo "log" >> out.log
来源：http://bqy.yangfankeji.com

[R41] 丢弃输出
来源：http://hdq.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://jtb.cheryme.top

[R42] 输入重定向
来源：http://yyu.zhengqikj.top

wc -l < a.txt
来源：http://fny.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://zed.xylfe.cn

find . -name "*.log" -type f
来源：http://ita.snrcjt.cn

[R44] 按修改时间查找
来源：http://inw.dashuyun.cn

find . -mtime -7 -type f
来源：http://tqp.cqqwz.cn

[R45] 批量删除
来源：http://put.svipenyu.cn

find . -name "*.tmp" -delete
来源：http://kua.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://oog.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wjv.vqdsnc.cn

[R47] sed 单行替换
来源：http://zfo.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://xsi.pengpengdd.cyou

[R48] awk 取指定列
来源：http://djc.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://wxw.316326.xyz

[R49] awk 带条件
来源：http://hti.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://edq.pengpengdd.cyou

[R50] awk 求和
来源：http://gzj.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mux.zycfv.cn

[R51] 排序去重取前几
来源：http://zgu.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://aqq.smart0.xyz

[R52] 统计行数
来源：http://uvi.sysykeji.top

wc -l a.txt
来源：http://lqj.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://bak.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cey.jinqigufen.top

[R54] 比较两个文件
来源：http://utr.nwbrower.top

diff a.txt b.txt
来源：http://wqa.jyoumei.cn

[R55] 压缩与解压
来源：http://gch.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nks.0kj1m.cn

[R56] 远程拷贝
来源：http://zfx.yueranfly.top

scp file user@host:/path/
来源：http://ger.316326.xyz

[R57] 远程执行命令
来源：http://wep.quarkkingdee.top

ssh user@host 'uptime'
来源：http://qnc.yfazqb.com

[R58] 下载文件
来源：http://gqa.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tij.tarul.cn

[R59] 发 POST JSON
来源：http://cxv.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rdv.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://afq.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wox.tanke756.top

[R61] 磁盘占用
来源：http://zec.bbcook.cn

df -h;  du -sh *
来源：http://zwk.hywenlv.cn

[R62] 找最占空间的文件
来源：http://akw.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://vpl.hysaishi.cn

[R63] 内存与进程
来源：http://cbn.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://pvx.jinghuilouyu.cn

[R64] 结束进程
来源：http://rhg.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://hof.guowangkeji.top

[R65] 查看端口占用
来源：http://xni.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://znw.vqdsnc.cn

[R66] 定时任务
来源：http://oya.jqgfzy.top

crontab -e;  crontab -l
来源：http://ycy.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://cty.meibo888.top

openssl rand -hex 16
来源：http://auq.yuxming.cn

[R68] 计算文件校验值
来源：http://nyf.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qqm.ehwqpu.com

[R69] 生成随机密码
来源：http://lrg.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://jzv.meibo888.top

[R70] 时间戳与互转
来源：http://crx.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://ytv.xylfe.cn

[R71] 日期格式化
来源：http://cst.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cnx.pycfn.com

[R72] 等待端口就绪
来源：http://qmg.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://aao.xuanzx.com

[R73] 分割大日志
来源：http://pmk.daria6918.cn

split -l 1000 big.log part_
来源：http://cfn.sxryk.cn

[R74] 批量重命名
来源：http://uxy.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ydg.pycfn.com

[R75] 导出环境变量
来源：http://zeh.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gwz.0kj1m.cn

[R76] 使用临时文件
来源：http://yyx.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kgl.fzhhl.top

[R77] 读取用户输入
来源：http://bra.hesvh.cn

read -rp "请输入: " ans
来源：http://wjt.jqgufenzy.top

[R78] 交互式菜单
来源：http://axx.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fmp.svipenyu.cn

[R79] 解析命令行选项
来源：http://rld.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rsd.tarul.cn

[R80] 查看脚本执行耗时
来源：http://cdy.jiagoushi.top

time ./run.sh
来源：http://mpy.epnwcf.com

================================================================================
来源：http://rhv.zdbjq.cn

S. C / C++ 专题
来源：http://iss.ctjpmb.com

================================================================================
来源：http://emy.iojbl.cn

[S01] C：Hello World
来源：http://hdd.hammf.cn

#include <stdio.h>
来源：http://ohp.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://txh.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://qzg.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://crb.nanxuanxn.top

[S03] C：读入整数
来源：http://rcf.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://wup.yj202588.top

[S04] C：字符串复制
来源：http://qug.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://elb.ybcxt.top

[S05] C：字符串长度
来源：http://wlg.hesvh.cn

strlen(s)
来源：http://ubg.c1oappe.top

[S06] C：字符串比较
来源：http://ymr.mhx1999.top

strcmp(a, b) == 0
来源：http://ymy.cqqwz.cn

[S07] C：数组遍历求和
来源：http://rmd.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://psg.316326.xyz

[S08] C：动态内存分配与释放
来源：http://fys.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zjm.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://cmu.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qbu.havefunace.top

[S10] C：指针与解引用
来源：http://ako.yueranfly.top

int *p = &a;  *p = 5;
来源：http://hjq.fktsv.cn

[S11] C：逐行读文件
来源：http://kmh.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://nlh.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ltq.zhengqikj.top

fclose(f);
来源：http://mgx.hfpthk.cn

[S12] C：写文件
来源：http://zpb.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ofz.jinqigufen.top

[S13] C：宏定义
来源：http://slu.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dpv.shuidangran.top

[S14] C：枚举
来源：http://ydi.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://juv.tarul.cn

[S15] C：类型转换
来源：http://zlp.zhaomingkeji.xyz

(double) a / b
来源：http://lan.kuanghao11.cn

[S16] C：位操作置位
来源：http://zjl.sjlbkw.cn

x |= (1 << 3);
来源：http://cex.yj202588.top

[S17] C：安全拼接字符串
来源：http://bwu.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://byz.hywenlv.cn

[S18] C：命令行参数
来源：http://ivy.xylfe.cn

int main(int argc, char **argv)
来源：http://fhp.hywenlv.cn

[S19] C：快速排序
来源：http://rql.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://cbk.yangfankeji.com

[S20] C：二分查找
来源：http://azi.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qzx.dianchejie.cn

[S21] C：字符类别判断
来源：http://ihs.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bvm.yonumen.top

[S22] C：字符串转数字
来源：http://fkn.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://bmb.dashuyun.cn

[S23] C：随机数
来源：http://ucl.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mri.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://fxc.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://umw.nanxuanxn.top

[S25] C：内存拷贝
来源：http://erw.yongpay.top

memcpy(dst, src, n);
来源：http://uwq.guowangkeji.top

[S26] C：内存清零
来源：http://kzc.xylfe.cn

memset(a, 0, sizeof a);
来源：http://lvr.ehwqpu.com

[S27] C：定义常量
来源：http://vbs.zycfv.cn

const double PI = 3.14159;
来源：http://awo.yuanzhike.top

[S28] C：静态变量
来源：http://nbv.cashguo.top

static int counter = 0;
来源：http://bmf.dianchejie.cn

[S29] C：变参函数
来源：http://zzp.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ssf.zdbjq.cn

[S30] C：头文件保护
来源：http://kky.meibo888.top

#ifndef X_H
来源：http://usp.316326.xyz

#define X_H
来源：http://vyz.fktsv.cn

#endif
来源：http://nmf.sxryk.cn

[S31] C++：Hello World
来源：http://ebg.fengsongda.top

#include <iostream>
来源：http://izh.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://whh.nanxuanxn.top

[S32] C++：字符串
来源：http://phu.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://emn.wangdashe.top

[S33] C++：vector 增删
来源：http://xcp.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pkh.yonumen.top

[S34] C++：遍历 vector
来源：http://syl.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://cxs.xinyue.icu

[S35] C++：map
来源：http://ldg.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rsw.ctjpmb.com

[S36] C++：unordered_map
来源：http://fdv.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uqe.gotoacloud.top

[S37] C++：set
来源：http://oqr.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://whr.sxryk.cn

[S38] C++：排序
来源：http://dcj.hammf.cn

std::sort(v.begin(), v.end());
来源：http://voi.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://ldz.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hqd.ppjwa.cn

[S40] C++：查找元素
来源：http://eje.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bvi.jiagoushi.top

[S41] C++：类与构造函数
来源：http://vnn.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oxw.yonumen.top

[S42] C++：继承与虚函数
来源：http://mon.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://bjf.daria6918.cn

[S43] C++：智能指针
来源：http://svd.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://bql.epnwcf.com

[S44] C++：引用传参
来源：http://lyj.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://upx.xingfuxueyuan.xyz


<!-- 参考信息 -->