代发 wailian999

[Q63] 开启事务
来源：http://kih.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yoz.yueranfly.top

[Q64] 提交事务
来源：http://nsa.gogol.net.cn

COMMIT;
来源：http://gmo.316326.xyz

[Q65] 回滚事务
来源：http://fsk.chenlongwang.top

ROLLBACK;
来源：http://gip.zdbjq.cn

[Q66] 行锁查询
来源：http://woa.cheryme.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwy.yj20258888.top

[Q67] 设置隔离级别
来源：http://ots.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://suk.wangdashe.top

[Q68] 保存点
来源：http://tzv.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://ssr.fengsongda.top

ROLLBACK TO sp1;
来源：http://jgc.tanke756.top

[Q69] 查看执行计划
来源：http://pxw.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rsa.gogol.net.cn

[Q70] 更新统计信息
来源：http://pjt.ydzc1.top

ANALYZE TABLE users;
来源：http://tst.hywenlv.cn

[Q71] 查看建表语句
来源：http://ofb.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vfn.pengpengdd.cyou

[Q72] 查看索引
来源：http://der.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://nvs.xuetiantiany.cn

[Q73] 查看表状态
来源：http://ejb.zhengqikj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xty.yangfankeji.com

[Q74] 强制使用索引
来源：http://drw.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ogb.quarkkingdee.top

[Q75] 日期格式化
来源：http://wnf.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://knh.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://laz.jinghuilouyu.cn

[Q76] 按天统计
来源：http://tnu.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wrm.hywenlv.cn

[Q77] 时间加减
来源：http://pqm.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mfh.zhengqikj.top

[Q78] 当前时间
来源：http://rvl.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qhe.iojbl.cn

[Q79] 字符串拼接
来源：http://mro.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://erp.iojbl.cn

[Q80] 字符串截取
来源：http://mie.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zfl.ydjk.org.cn

[Q81] 字符串替换
来源：http://vng.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nye.shangyingyoupin.top

[Q82] 字符长度与字节长度
来源：http://hzn.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://akv.svipenyu.cn

[Q83] 大小写转换
来源：http://vjj.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kew.yueranfly.top

[Q84] 去除首尾空格
来源：http://gww.xinyue.icu

SELECT TRIM(name) FROM users;
来源：http://vla.nanxuanxn.top

[Q85] 数值取整
来源：http://gln.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bms.zhijiandao.cn

[Q86] 读取 JSON 字段
来源：http://hpv.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mst.uphjek.com

[Q87] JSON 字段做条件
来源：http://qbi.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gny.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://hmc.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dxm.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ygi.andypj.xyz

[Q89] 判断表是否存在
来源：http://wis.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oof.feifeiyinyue.top

[Q90] 生成序号列
来源：http://mjx.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lqz.yj202588.top

================================================================================
来源：http://xgw.cqqwz.cn

R. Bash 专题
来源：http://xoc.cqqwz.cn

================================================================================
来源：http://cje.fktsv.cn

[R01] shebang 与严格模式
来源：http://vaw.sxryk.cn

#!/usr/bin/env bash
来源：http://ffz.sjlbkw.cn

set -euo pipefail
来源：http://avu.cqqwz.cn

[R02] 变量赋值与使用
来源：http://jlk.tarul.cn

name="Tom"; echo "$name"
来源：http://alk.pycfn.com

[R03] 只读变量
来源：http://sth.gogol.net.cn

readonly PI=3.14
来源：http://ogb.gzhubu.top

[R04] 位置参数
来源：http://ggo.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bah.dashuyun.cn

[R05] 参数默认值
来源：http://nbi.jianghu66.top

name="${1:-default}"
来源：http://uol.fktsv.cn

[R06] 判断命令是否存在
来源：http://mvf.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hus.fehbvm.com

[R07] if 判断文件
来源：http://ost.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gcb.dashuyun.cn

[R08] 数值比较
来源：http://weg.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vvz.aibaodan.cn

[R09] 字符串比较
来源：http://nbr.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zdh.fengsongda.top

[R10] 正则匹配
来源：http://val.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hdo.yangfankeji.com

[R11] case 多分支
来源：http://nbi.zhaomingkeji.xyz

case "$1" in
来源：http://yfo.svipenyu.cn

start) echo "启动" ;;
来源：http://idq.9152youxi.cn

stop)  echo "停止" ;;
来源：http://mby.yongpay.top

*)     echo "未知命令" ;;
来源：http://dwq.jqgufenzy.top

esac
来源：http://kin.jqgfzy.top

[R12] for 遍历文件
来源：http://cpz.ybcxt.top

for f in *.txt; do echo "$f"; done
来源：http://zxs.cashguo.top

[R13] for 计数循环
来源：http://xyx.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://mgr.sjlbkw.cn

[R14] C 风格 for
来源：http://fzk.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dku.vehdjk.com

[R15] while 逐行读文件
来源：http://uws.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vvf.smart0.xyz

[R16] until 等待条件
来源：http://epr.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ayb.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://vnk.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vza.gzhubu.top

[R18] 遍历数组
来源：http://tuw.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fps.feifeiyinyue.top

[R19] 数组长度
来源：http://cyh.cashguo.top

echo "${#arr[@]}"
来源：http://smx.zhixingplan.top

[R20] 关联数组（字典）
来源：http://kbk.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://owy.yvedp.cn

[R21] 字符串长度
来源：http://odk.hammf.cn

echo "${#s}"
来源：http://vzq.feifeiyinyue.top

[R22] 截取子串
来源：http://qkl.nwbrower.top

echo "${s:0:5}"
来源：http://hre.ivvv.top

[R23] 字符串替换
来源：http://rab.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nfz.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://htr.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://mru.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://cmf.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qdi.jiagoushi.top

[R26] 命令替换
来源：http://rtq.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://hcx.9152youxi.cn

[R27] 算术展开
来源：http://xja.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://hpp.sweek.top

[R28] 浮点运算
来源：http://nmv.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://uou.fengsongda.top

[R29] 定义函数
来源：http://ctn.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qlj.yangfankeji.com

[R30] 函数返回状态码
来源：http://eic.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://hus.tianlin.xyz

[R31] 局部变量
来源：http://gog.sweek.top

f() { local x=1; echo "$x"; }
来源：http://xmh.ybcxt.top

[R32] 参数个数校验
来源：http://pug.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qpe.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://jug.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ohg.feifeiyinyue.top

[R34] 退出时清理
来源：http://qsl.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xrj.sxryk.cn

[R35] 后台执行并等待
来源：http://imu.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://zdt.chenlongwang.top

[R36] 并发执行多个任务
来源：http://xfe.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yrw.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://rou.yueranfly.top

files=$(ls -1)
来源：http://mai.pycfn.com

[R38] 管道串联
来源：http://str.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://xzx.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://dwu.cdnleiting.top

cmd > out.log 2>&1
来源：http://jrx.haohaochexian.top

[R40] 追加写日志
来源：http://sbx.zdqjudy.top

echo "log" >> out.log
来源：http://szh.gaohongyu789.top

[R41] 丢弃输出
来源：http://ccv.xylfe.cn

cmd >/dev/null 2>&1
来源：http://oam.zhoulong.xyz

[R42] 输入重定向
来源：http://tee.bjfxy.top

wc -l < a.txt
来源：http://vay.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://iwa.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://iea.yongpay.top

[R44] 按修改时间查找
来源：http://niv.gogol.net.cn

find . -mtime -7 -type f
来源：http://obc.bbcook.cn

[R45] 批量删除
来源：http://emq.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://rbz.daxiang520.top

[R46] 递归替换文件内容
来源：http://mme.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cwt.chenlongwang.top

[R47] sed 单行替换
来源：http://uke.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://oir.316326.xyz

[R48] awk 取指定列
来源：http://lhj.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://gfx.hongshengwenyu.top

[R49] awk 带条件
来源：http://kcs.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vzx.tian-w.cn

[R50] awk 求和
来源：http://yrw.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://bfo.gzhubu.top

[R51] 排序去重取前几
来源：http://ber.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iow.yfazqb.com

[R52] 统计行数
来源：http://udd.jinqigfzy.top

wc -l a.txt
来源：http://kxk.sweek.top

[R53] 查看文件头与实时尾
来源：http://axe.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wzh.sweek.top

[R54] 比较两个文件
来源：http://yit.mhx1999.top

diff a.txt b.txt
来源：http://whh.nanxuanxn.top

[R55] 压缩与解压
来源：http://fya.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eis.zhongyouzk.top

[R56] 远程拷贝
来源：http://uoz.shuidangran.top

scp file user@host:/path/
来源：http://ztz.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://zuf.yongpay.top

ssh user@host 'uptime'
来源：http://hso.ydzc1.top

[R58] 下载文件
来源：http://qzv.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cdp.hywenlv.cn

[R59] 发 POST JSON
来源：http://heh.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ioy.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://bxi.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bco.hammf.cn

[R61] 磁盘占用
来源：http://hzp.svipenyu.cn

df -h;  du -sh *
来源：http://aji.chenlongwang.top

[R62] 找最占空间的文件
来源：http://rzf.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://ykj.zdqjudy.top

[R63] 内存与进程
来源：http://jzw.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://mbj.zdqjudy.top

[R64] 结束进程
来源：http://hlv.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://pca.jianghu66.top

[R65] 查看端口占用
来源：http://dqr.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://djs.yonumen.top

[R66] 定时任务
来源：http://hrz.gzhubu.top

crontab -e;  crontab -l
来源：http://vjj.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://pzn.jlsjyb.cn

openssl rand -hex 16
来源：http://jtw.sufxvd.cn

[R68] 计算文件校验值
来源：http://bpq.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://rxo.yongpay.top

[R69] 生成随机密码
来源：http://ynz.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://xvb.tanke756.top

[R70] 时间戳与互转
来源：http://ajb.yongpay.top

date +%s;  date -d @1700000000
来源：http://xmw.bbcook.cn

[R71] 日期格式化
来源：http://hna.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://mou.yj202588.top

[R72] 等待端口就绪
来源：http://yco.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zdm.sweek.top

[R73] 分割大日志
来源：http://nhp.cucudq.cn

split -l 1000 big.log part_
来源：http://riy.vqdsnc.cn

[R74] 批量重命名
来源：http://ald.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jbw.quarkkingdee.top

[R75] 导出环境变量
来源：http://egh.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://kli.hammf.cn

[R76] 使用临时文件
来源：http://bqb.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://osh.dianchejie.cn

[R77] 读取用户输入
来源：http://wrk.hesvh.cn

read -rp "请输入: " ans
来源：http://ecc.uphjek.com

[R78] 交互式菜单
来源：http://zyd.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wjc.birdmap.top

[R79] 解析命令行选项
来源：http://fhx.dashuyun.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://prn.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://bph.sysykeji.top

time ./run.sh
来源：http://agd.bjfxy.top

================================================================================
来源：http://gcb.mhx1999.top

S. C / C++ 专题
来源：http://hmw.zdbjq.cn

================================================================================
来源：http://sbx.yj20258888.top

[S01] C：Hello World
来源：http://ciy.ybcxt.top

#include <stdio.h>
来源：http://qxd.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pjt.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://eam.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://lbk.zhixingplan.top

[S03] C：读入整数
来源：http://mbi.sufxvd.cn

int x; scanf("%d", &x);
来源：http://fny.daria6918.cn

[S04] C：字符串复制
来源：http://ehr.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://qai.wangshuangyany.cn

[S05] C：字符串长度
来源：http://mtc.shangyingyoupin.top

strlen(s)
来源：http://prj.zycfv.cn

[S06] C：字符串比较
来源：http://fqh.guowangkeji.top

strcmp(a, b) == 0
来源：http://mwb.zycfv.cn

[S07] C：数组遍历求和
来源：http://ljk.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hzu.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://uep.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eef.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://fvk.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uwl.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://duf.sysykeji.top

int *p = &a;  *p = 5;
来源：http://tza.vehdjk.com

[S11] C：逐行读文件
来源：http://osp.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://dnk.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ysh.feifeiyinyue.top

fclose(f);
来源：http://vmp.jqgufenzy.top

[S12] C：写文件
来源：http://yzp.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kfz.jqgufenzy.top

[S13] C：宏定义
来源：http://njn.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://grk.epnwcf.com

[S14] C：枚举
来源：http://kpp.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://zwy.yongpay.top

[S15] C：类型转换
来源：http://vsn.hammf.cn

(double) a / b
来源：http://oly.jlsjyb.cn

[S16] C：位操作置位
来源：http://tbe.jiagoushi.top

x |= (1 << 3);
来源：http://viq.ybcxt.top

[S17] C：安全拼接字符串
来源：http://fsc.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://plr.redwolf501.top

[S18] C：命令行参数
来源：http://nzb.svipenyu.cn

int main(int argc, char **argv)
来源：http://vja.chenzaomai.com

[S19] C：快速排序
来源：http://jpw.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://mnd.sxryk.cn

[S20] C：二分查找
来源：http://hyf.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kis.sufxvd.cn

[S21] C：字符类别判断
来源：http://cld.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cal.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://dey.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iwq.zhiwuduotai.top

[S23] C：随机数
来源：http://jng.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yjp.c1oappe.top

[S24] C：获取本地时间
来源：http://tzq.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jff.hammf.cn

[S25] C：内存拷贝
来源：http://cqi.tianlin.xyz

memcpy(dst, src, n);
来源：http://jbw.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://cff.nwbrower.top

memset(a, 0, sizeof a);
来源：http://xvj.vqdsnc.cn

[S27] C：定义常量
来源：http://whp.ydzc1.top

const double PI = 3.14159;
来源：http://krg.yueranfly.top

[S28] C：静态变量
来源：http://ued.xingfuxueyuan.xyz

static int counter = 0;
来源：http://esm.nanxuanxn.top

[S29] C：变参函数
来源：http://rry.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmg.uphjek.com

[S30] C：头文件保护
来源：http://mks.feifeiyinyue.top

#ifndef X_H
来源：http://spd.pengpengdd.cyou

#define X_H
来源：http://jig.9152youxi.cn

#endif
来源：http://zjo.wangdashe.top

[S31] C++：Hello World
来源：http://xxu.fengsongda.top

#include <iostream>
来源：http://fid.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://acg.aibaodan.cn

[S32] C++：字符串
来源：http://aoq.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://jcf.xuanzx.com


<!-- 参考信息 -->