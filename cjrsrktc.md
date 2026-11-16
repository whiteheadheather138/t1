代发 wailian999

[Q67] 设置隔离级别
来源：http://kvk.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zly.cheryme.top

[Q68] 保存点
来源：http://eli.hcnkem.com

SAVEPOINT sp1;
来源：http://twg.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ret.cdnleiting.top

[Q69] 查看执行计划
来源：http://auh.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dhw.daxiang520.top

[Q70] 更新统计信息
来源：http://fon.yongpay.top

ANALYZE TABLE users;
来源：http://qwl.hywenlv.cn

[Q71] 查看建表语句
来源：http://zrn.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xbw.tianlin.xyz

[Q72] 查看索引
来源：http://xqx.smart0.xyz

SHOW INDEX FROM users;
来源：http://zrt.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://lpi.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qcz.fzhhl.top

[Q74] 强制使用索引
来源：http://glq.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://brv.zdqjudy.top

[Q75] 日期格式化
来源：http://wag.fanxiaobao.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ids.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://djh.jqgufenzy.top

[Q76] 按天统计
来源：http://knh.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jwp.tarul.cn

[Q77] 时间加减
来源：http://drw.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uxy.kuanghao11.cn

[Q78] 当前时间
来源：http://mhd.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kwo.gaohongyu789.top

[Q79] 字符串拼接
来源：http://wox.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://foh.pengpengdd.cyou

[Q80] 字符串截取
来源：http://zih.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kqs.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://zsd.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uma.quarkkingdee.top

[Q82] 字符长度与字节长度
来源：http://mav.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://she.tarul.cn

[Q83] 大小写转换
来源：http://jby.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://roh.zhengqikj.top

[Q84] 去除首尾空格
来源：http://piz.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://kpu.hammf.cn

[Q85] 数值取整
来源：http://rlt.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bct.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://qjs.gzhubu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qvp.yonumen.top

[Q87] JSON 字段做条件
来源：http://wbw.yanxiufei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jgv.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://hpr.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dud.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jmg.yvedp.cn

[Q89] 判断表是否存在
来源：http://vro.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ywy.uphjek.com

[Q90] 生成序号列
来源：http://oku.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://map.pengpengdd.cyou

================================================================================
来源：http://vwe.gaohongyu789.top

R. Bash 专题
来源：http://vfp.vqdsnc.cn

================================================================================
来源：http://yjw.cdnleiting.top

[R01] shebang 与严格模式
来源：http://czl.zhongyouzk.top

#!/usr/bin/env bash
来源：http://uxr.zhongyouzk.top

set -euo pipefail
来源：http://ppc.cashguo.top

[R02] 变量赋值与使用
来源：http://myl.wangdashe.top

name="Tom"; echo "$name"
来源：http://ekr.ydjk.org.cn

[R03] 只读变量
来源：http://rvw.sxryk.cn

readonly PI=3.14
来源：http://nhg.bjfxy.top

[R04] 位置参数
来源：http://urq.vehdjk.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zze.yj20258888.top

[R05] 参数默认值
来源：http://tkh.snrcjt.cn

name="${1:-default}"
来源：http://pop.jqgfzy.top

[R06] 判断命令是否存在
来源：http://xhs.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lof.aibaodan.cn

[R07] if 判断文件
来源：http://jlp.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ruk.guannengcc.top

[R08] 数值比较
来源：http://yuo.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uie.nanxuanxn.top

[R09] 字符串比较
来源：http://zff.guannengcc.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mok.ppjwa.cn

[R10] 正则匹配
来源：http://jyw.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jst.ppjwa.cn

[R11] case 多分支
来源：http://aqr.yanxiufei.cn

case "$1" in
来源：http://fqz.gaohongyu789.top

start) echo "启动" ;;
来源：http://mjv.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://tus.aizwys.cn

*)     echo "未知命令" ;;
来源：http://rbv.smart0.xyz

esac
来源：http://bbo.yfazqb.com

[R12] for 遍历文件
来源：http://ike.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://hgq.ivvv.top

[R13] for 计数循环
来源：http://oxs.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://mwn.hywenlv.cn

[R14] C 风格 for
来源：http://fjw.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xmp.fzhhl.top

[R15] while 逐行读文件
来源：http://kpp.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pcv.yangfankeji.com

[R16] until 等待条件
来源：http://emp.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://obt.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://fqm.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://ijg.yangfankeji.com

[R18] 遍历数组
来源：http://lbq.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hxj.gaohongyu789.top

[R19] 数组长度
来源：http://gcd.0kj1m.cn

echo "${#arr[@]}"
来源：http://qpt.daxiang520.top

[R20] 关联数组（字典）
来源：http://icr.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kjl.bbcook.cn

[R21] 字符串长度
来源：http://xzg.shanyushiyangkeji.top

echo "${#s}"
来源：http://tzr.yuxming.cn

[R22] 截取子串
来源：http://xrw.316326.xyz

echo "${s:0:5}"
来源：http://bip.uphjek.com

[R23] 字符串替换
来源：http://qih.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hnh.zhiwuduotai.top

[R24] 大小写转换
来源：http://wob.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://mlv.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://pxx.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ivk.9152youxi.cn

[R26] 命令替换
来源：http://zng.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://bhz.bbcook.cn

[R27] 算术展开
来源：http://nnm.zycfv.cn

echo $((1 + 2 * 3))
来源：http://dlb.zhiwuduotai.top

[R28] 浮点运算
来源：http://ydv.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://fbv.c1oappe.top

[R29] 定义函数
来源：http://hyg.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dok.zhijiandao.cn

[R30] 函数返回状态码
来源：http://tbd.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://zoh.gaohongyu789.top

[R31] 局部变量
来源：http://uqx.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://szr.haohaochexian.top

[R32] 参数个数校验
来源：http://buj.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wij.yonumen.top

[R33] 捕获错误并提示行号
来源：http://noz.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tql.dianchejie.cn

[R34] 退出时清理
来源：http://bjo.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://epm.gotoacloud.top

[R35] 后台执行并等待
来源：http://qqi.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cxt.gotoacloud.top

[R36] 并发执行多个任务
来源：http://ahd.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bca.xinyue.icu

[R37] 把输出赋给变量
来源：http://kec.tarul.cn

files=$(ls -1)
来源：http://xxp.tarul.cn

[R38] 管道串联
来源：http://owu.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://txp.cashguo.top

[R39] 重定向标准输出与错误
来源：http://pth.cucudq.cn

cmd > out.log 2>&1
来源：http://zqj.hammf.cn

[R40] 追加写日志
来源：http://lrv.yangfankeji.com

echo "log" >> out.log
来源：http://uxv.jinqigufen.top

[R41] 丢弃输出
来源：http://xhu.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://mhj.hywenlv.cn

[R42] 输入重定向
来源：http://mxc.xziqi.cn

wc -l < a.txt
来源：http://chu.yuanzhike.top

[R43] 按名字查找文件
来源：http://lmf.yuanzhike.top

find . -name "*.log" -type f
来源：http://tef.hnxiangtu.top

[R44] 按修改时间查找
来源：http://hqs.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://qwm.gaohongyu789.top

[R45] 批量删除
来源：http://qiz.316326.xyz

find . -name "*.tmp" -delete
来源：http://lpd.hcnkem.com

[R46] 递归替换文件内容
来源：http://yct.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mba.52xcode.cn

[R47] sed 单行替换
来源：http://udu.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ojk.ydzc1.top

[R48] awk 取指定列
来源：http://xrk.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://uiq.zhixingplan.top

[R49] awk 带条件
来源：http://ivo.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dci.jlsjyb.cn

[R50] awk 求和
来源：http://kag.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hoh.xziqi.cn

[R51] 排序去重取前几
来源：http://xpv.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oqe.jianghu66.top

[R52] 统计行数
来源：http://jxw.shanyushiyangkeji.top

wc -l a.txt
来源：http://nmf.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://stv.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fis.hammf.cn

[R54] 比较两个文件
来源：http://vkw.nwbrower.top

diff a.txt b.txt
来源：http://ywi.zdqjudy.top

[R55] 压缩与解压
来源：http://ajq.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qyx.tianlin.xyz

[R56] 远程拷贝
来源：http://unh.cdnleiting.top

scp file user@host:/path/
来源：http://jdm.aizwys.cn

[R57] 远程执行命令
来源：http://gbv.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://lrc.guannengcc.top

[R58] 下载文件
来源：http://tcf.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ycl.zhijiandao.cn

[R59] 发 POST JSON
来源：http://kul.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skc.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://abr.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iee.yongpay.top

[R61] 磁盘占用
来源：http://iac.hysaishi.cn

df -h;  du -sh *
来源：http://ozw.zdbjq.cn

[R62] 找最占空间的文件
来源：http://ssk.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://eih.chenzaomai.com

[R63] 内存与进程
来源：http://wga.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://odh.pengpengdd.cyou

[R64] 结束进程
来源：http://bms.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://tuv.bbcook.cn

[R65] 查看端口占用
来源：http://rbn.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mxv.yuxming.cn

[R66] 定时任务
来源：http://xxf.gzhubu.top

crontab -e;  crontab -l
来源：http://kbm.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://kcc.yongpay.top

openssl rand -hex 16
来源：http://vdj.hywenlv.cn

[R68] 计算文件校验值
来源：http://aia.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://izc.hfpthk.cn

[R69] 生成随机密码
来源：http://dxe.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://edu.zdbjq.cn

[R70] 时间戳与互转
来源：http://lth.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://jdj.gogol.net.cn

[R71] 日期格式化
来源：http://dvp.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uhl.jiagoushi.top

[R72] 等待端口就绪
来源：http://cpm.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qqi.haohaochexian.top

[R73] 分割大日志
来源：http://oxo.nanxuanxn.top

split -l 1000 big.log part_
来源：http://lnf.quarkkingdee.top

[R74] 批量重命名
来源：http://kqs.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hco.316326.xyz

[R75] 导出环境变量
来源：http://ale.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://avp.xuanzx.com

[R76] 使用临时文件
来源：http://dqd.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lot.epnwcf.com

[R77] 读取用户输入
来源：http://pev.zdqjudy.top

read -rp "请输入: " ans
来源：http://htv.ivvv.top

[R78] 交互式菜单
来源：http://yck.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://uee.hcnkem.com

[R79] 解析命令行选项
来源：http://rhj.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gbn.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://cec.xziqi.cn

time ./run.sh
来源：http://yhp.sysykeji.top

================================================================================
来源：http://pip.yanxiufei.cn

S. C / C++ 专题
来源：http://syh.sjlbkw.cn

================================================================================
来源：http://ncl.chenlongwang.top

[S01] C：Hello World
来源：http://moo.ehwqpu.com

#include <stdio.h>
来源：http://vvq.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ijh.epnwcf.com

[S02] C：变量与格式化输出
来源：http://kpf.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://uxf.yj20258888.top

[S03] C：读入整数
来源：http://kro.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://rgt.cqqwz.cn

[S04] C：字符串复制
来源：http://rfx.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dlp.yvedp.cn

[S05] C：字符串长度
来源：http://qhn.fktsv.cn

strlen(s)
来源：http://pmj.fengsongda.top

[S06] C：字符串比较
来源：http://wcq.pycfn.com

strcmp(a, b) == 0
来源：http://nsi.yfazqb.com

[S07] C：数组遍历求和
来源：http://fry.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wxt.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://jcm.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cep.gogol.net.cn

[S09] C：结构体定义与初始化
来源：http://lod.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tlr.xuanzx.com

[S10] C：指针与解引用
来源：http://iur.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://kyh.zhengqikj.top

[S11] C：逐行读文件
来源：http://hyl.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://iea.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uia.hammf.cn

fclose(f);
来源：http://jmo.zhengqikj.top

[S12] C：写文件
来源：http://icq.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lvm.xuetiantiany.cn

[S13] C：宏定义
来源：http://rzg.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bih.zhaomingkeji.xyz

[S14] C：枚举
来源：http://itt.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://nog.jlsjyb.cn

[S15] C：类型转换
来源：http://lbr.uphjek.com

(double) a / b
来源：http://ewq.jinqigfzy.top

[S16] C：位操作置位
来源：http://uhl.yonumen.top

x |= (1 << 3);
来源：http://dxb.xylfe.cn

[S17] C：安全拼接字符串
来源：http://pqc.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktq.zdbjq.cn

[S18] C：命令行参数
来源：http://mej.dashuyun.cn

int main(int argc, char **argv)
来源：http://qcr.gogol.net.cn

[S19] C：快速排序
来源：http://osn.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tec.ehwqpu.com

[S20] C：二分查找
来源：http://dwq.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rkq.zdqjudy.top

[S21] C：字符类别判断
来源：http://ffn.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dps.guowangkeji.top

[S22] C：字符串转数字
来源：http://uln.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://wqj.zhixingplan.top

[S23] C：随机数
来源：http://fgn.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vgb.hcnkem.com

[S24] C：获取本地时间
来源：http://ott.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tav.haohaochexian.top

[S25] C：内存拷贝
来源：http://kyh.zhengqikj.top

memcpy(dst, src, n);
来源：http://lke.yj20258888.top

[S26] C：内存清零
来源：http://eji.xziqi.cn

memset(a, 0, sizeof a);
来源：http://cuc.mhx1999.top

[S27] C：定义常量
来源：http://zgx.pengpengdd.cyou

const double PI = 3.14159;
来源：http://qsj.hammf.cn

[S28] C：静态变量
来源：http://pix.gotoacloud.top

static int counter = 0;
来源：http://dbx.zhengqikj.top

[S29] C：变参函数
来源：http://woj.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jcv.yongpay.top

[S30] C：头文件保护
来源：http://hmk.yueranfly.top

#ifndef X_H
来源：http://jkh.hywenlv.cn

#define X_H
来源：http://vzl.yj20258.top

#endif
来源：http://iod.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://gzq.sysykeji.top

#include <iostream>
来源：http://dgr.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://zkj.yonumen.top

[S32] C++：字符串
来源：http://knd.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://zzu.kuanghao11.cn

[S33] C++：vector 增删
来源：http://htw.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nma.hcnkem.com

[S34] C++：遍历 vector
来源：http://rio.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://ptb.haohaochexian.top

[S35] C++：map
来源：http://wsm.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jqe.ivvv.top

[S36] C++：unordered_map
来源：http://mqp.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ygp.nanxuanxn.top


<!-- 参考信息 -->