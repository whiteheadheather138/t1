代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zgk.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://wku.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vwm.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngj.fzhhl.top

[Q61] 移动平均
来源：http://tws.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ouc.9152youxi.cn

[Q62] 分组占比
来源：http://vcv.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nvb.zycfv.cn

[Q63] 开启事务
来源：http://xui.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://loc.shuidangran.top

[Q64] 提交事务
来源：http://yce.gotoacloud.top

COMMIT;
来源：http://jee.dianchejie.cn

[Q65] 回滚事务
来源：http://xrq.hnqzz.top

ROLLBACK;
来源：http://ykq.c1oappe.top

[Q66] 行锁查询
来源：http://zyh.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ctv.yvedp.cn

[Q67] 设置隔离级别
来源：http://vol.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nxi.jinghuilouyu.cn

[Q68] 保存点
来源：http://tjd.yangfankeji.com

SAVEPOINT sp1;
来源：http://kop.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://pxm.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://rhp.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zua.ppjwa.cn

[Q70] 更新统计信息
来源：http://voa.shuidangran.top

ANALYZE TABLE users;
来源：http://tug.yanxiufei.cn

[Q71] 查看建表语句
来源：http://vgp.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mqb.c1oappe.top

[Q72] 查看索引
来源：http://ngo.wangdashe.top

SHOW INDEX FROM users;
来源：http://cdm.cqqwz.cn

[Q73] 查看表状态
来源：http://npa.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://lbf.dashuyun.cn

[Q74] 强制使用索引
来源：http://vkm.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yrl.sxryk.cn

[Q75] 日期格式化
来源：http://zsm.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yfe.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://awv.zhiwuduotai.top

[Q76] 按天统计
来源：http://xse.yfazqb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pxa.cdnleiting.top

[Q77] 时间加减
来源：http://zmp.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fcm.c1oappe.top

[Q78] 当前时间
来源：http://uws.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mlh.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://zql.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wja.yvedp.cn

[Q80] 字符串截取
来源：http://fsd.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ula.dianchejie.cn

[Q81] 字符串替换
来源：http://okf.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tqm.zdqjudy.top

[Q82] 字符长度与字节长度
来源：http://vzw.zhiwuduotai.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://duq.xinyue.icu

[Q83] 大小写转换
来源：http://wll.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fwh.uphjek.com

[Q84] 去除首尾空格
来源：http://ldq.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://bii.guowangkeji.top

[Q85] 数值取整
来源：http://neh.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ayu.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://zxf.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oge.fengsongda.top

[Q87] JSON 字段做条件
来源：http://qeo.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xqe.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://sgs.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vwo.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kiw.jqgfzy.top

[Q89] 判断表是否存在
来源：http://kdx.svipenyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vui.zhoulong.xyz

[Q90] 生成序号列
来源：http://lza.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://snx.pengpengdd.cyou

================================================================================
来源：http://sji.hcnkem.com

R. Bash 专题
来源：http://eeb.epnwcf.com

================================================================================
来源：http://qkx.chenzaomai.com

[R01] shebang 与严格模式
来源：http://yhw.wangdashe.top

#!/usr/bin/env bash
来源：http://wip.jyoumei.cn

set -euo pipefail
来源：http://bdx.ppjwa.cn

[R02] 变量赋值与使用
来源：http://yfu.yueranfly.top

name="Tom"; echo "$name"
来源：http://plz.hesvh.cn

[R03] 只读变量
来源：http://ksw.chenzaomai.com

readonly PI=3.14
来源：http://dem.yanxiufei.cn

[R04] 位置参数
来源：http://wna.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jhw.pycfn.com

[R05] 参数默认值
来源：http://gij.chenjidiqi.icu

name="${1:-default}"
来源：http://hzl.daxiang520.top

[R06] 判断命令是否存在
来源：http://yqp.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nga.ydjk.org.cn

[R07] if 判断文件
来源：http://xgd.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qpy.yonumen.top

[R08] 数值比较
来源：http://qpc.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dzo.mhx1999.top

[R09] 字符串比较
来源：http://cig.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jba.daxiang520.top

[R10] 正则匹配
来源：http://mmg.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jnd.zhongyouzk.top

[R11] case 多分支
来源：http://ibv.snrcjt.cn

case "$1" in
来源：http://vwx.wangshuangyany.cn

start) echo "启动" ;;
来源：http://sxh.zhixingplan.top

stop)  echo "停止" ;;
来源：http://tyd.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://bpy.shanyushiyangtech.top

esac
来源：http://kmz.hywenlv.cn

[R12] for 遍历文件
来源：http://knz.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://gll.c1oappe.top

[R13] for 计数循环
来源：http://rza.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://sbk.xziqi.cn

[R14] C 风格 for
来源：http://qyj.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mjw.pycfn.com

[R15] while 逐行读文件
来源：http://tjo.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mnj.cucudq.cn

[R16] until 等待条件
来源：http://xrk.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lmw.zycfv.cn

[R17] 数组定义与取值
来源：http://yyw.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://pli.fehbvm.com

[R18] 遍历数组
来源：http://mcz.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dpn.daxiang520.top

[R19] 数组长度
来源：http://gym.guowangkeji.top

echo "${#arr[@]}"
来源：http://tsf.hfpthk.cn

[R20] 关联数组（字典）
来源：http://gbm.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jhp.snrcjt.cn

[R21] 字符串长度
来源：http://frt.yueranfly.top

echo "${#s}"
来源：http://gcs.smart0.xyz

[R22] 截取子串
来源：http://mjb.wangshuangyany.cn

echo "${s:0:5}"
来源：http://kjl.xuanzx.com

[R23] 字符串替换
来源：http://kan.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zzl.tian-w.cn

[R24] 大小写转换
来源：http://jot.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://yig.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://tai.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mhh.smart0.xyz

[R26] 命令替换
来源：http://bzd.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://yal.bjfxy.top

[R27] 算术展开
来源：http://hqg.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://ocq.zhengqikj.top

[R28] 浮点运算
来源：http://qdo.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://hcf.xinyue.icu

[R29] 定义函数
来源：http://nmo.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bkv.cqqwz.cn

[R30] 函数返回状态码
来源：http://mrw.ppjwa.cn

f() { return 0; }; f || echo "失败了"
来源：http://hnb.sjlbkw.cn

[R31] 局部变量
来源：http://ksh.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://obo.hongshengwenyu.top

[R32] 参数个数校验
来源：http://uwo.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ybv.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://sxz.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xoo.zhongyouzk.top

[R34] 退出时清理
来源：http://bgl.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cmh.hnxiangtu.top

[R35] 后台执行并等待
来源：http://ezk.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zgm.sxryk.cn

[R36] 并发执行多个任务
来源：http://dho.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zku.zhengqikj.top

[R37] 把输出赋给变量
来源：http://fwv.zdqjudy.top

files=$(ls -1)
来源：http://xhs.hnxiangtu.top

[R38] 管道串联
来源：http://uwe.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://ocs.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://fwk.nwbrower.top

cmd > out.log 2>&1
来源：http://akt.bbcook.cn

[R40] 追加写日志
来源：http://tds.fzhhl.top

echo "log" >> out.log
来源：http://rkw.jinqigfzy.top

[R41] 丢弃输出
来源：http://wgw.tanke756.top

cmd >/dev/null 2>&1
来源：http://ack.iojbl.cn

[R42] 输入重定向
来源：http://run.zycfv.cn

wc -l < a.txt
来源：http://pcx.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://mvi.yangfankeji.com

find . -name "*.log" -type f
来源：http://qfq.jinqigufen.top

[R44] 按修改时间查找
来源：http://jvg.316326.xyz

find . -mtime -7 -type f
来源：http://vpa.andypj.xyz

[R45] 批量删除
来源：http://mrz.vehdjk.com

find . -name "*.tmp" -delete
来源：http://szg.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://tjh.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://opm.pengpengdd.cyou

[R47] sed 单行替换
来源：http://kkb.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://hwh.chenlongwang.top

[R48] awk 取指定列
来源：http://vpe.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://vrt.daria6918.cn

[R49] awk 带条件
来源：http://txc.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vfs.dashuyun.cn

[R50] awk 求和
来源：http://fco.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://kpe.hcnkem.com

[R51] 排序去重取前几
来源：http://qen.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tuh.jyoumei.cn

[R52] 统计行数
来源：http://dor.zhixingplan.top

wc -l a.txt
来源：http://zlk.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://jyg.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ytc.9152youxi.cn

[R54] 比较两个文件
来源：http://pik.gotoacloud.top

diff a.txt b.txt
来源：http://qnn.nanxinkj.top

[R55] 压缩与解压
来源：http://dac.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sqc.fengsongda.top

[R56] 远程拷贝
来源：http://jjp.yj20258888.top

scp file user@host:/path/
来源：http://tda.xuanzx.com

[R57] 远程执行命令
来源：http://rkd.jqgfzy.top

ssh user@host 'uptime'
来源：http://yit.zdqjudy.top

[R58] 下载文件
来源：http://anc.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fqh.hywenlv.cn

[R59] 发 POST JSON
来源：http://jux.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://etx.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://jge.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kyq.tianlin.xyz

[R61] 磁盘占用
来源：http://pii.tianlin.xyz

df -h;  du -sh *
来源：http://mjk.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://kwb.birdmap.top

du -ah . | sort -rh | head -10
来源：http://cfl.zhixingplan.top

[R63] 内存与进程
来源：http://ltv.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://kcm.iojbl.cn

[R64] 结束进程
来源：http://tjs.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://zvb.hammf.cn

[R65] 查看端口占用
来源：http://lni.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nnu.svipenyu.cn

[R66] 定时任务
来源：http://jog.xuanzx.com

crontab -e;  crontab -l
来源：http://ftv.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://rxd.epnwcf.com

openssl rand -hex 16
来源：http://vdj.snrcjt.cn

[R68] 计算文件校验值
来源：http://csj.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://dhv.hammf.cn

[R69] 生成随机密码
来源：http://pmb.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://qen.zhixingplan.top

[R70] 时间戳与互转
来源：http://ipp.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://ebu.jinqigufen.top

[R71] 日期格式化
来源：http://qmu.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lgl.sufxvd.cn

[R72] 等待端口就绪
来源：http://vfn.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sha.fehbvm.com

[R73] 分割大日志
来源：http://zec.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://qrp.shangyingyoupin.top

[R74] 批量重命名
来源：http://qfo.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xbz.fktsv.cn

[R75] 导出环境变量
来源：http://loo.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://fwm.yonumen.top

[R76] 使用临时文件
来源：http://sxa.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://stw.guowangkeji.top

[R77] 读取用户输入
来源：http://qmv.zhoulong.xyz

read -rp "请输入: " ans
来源：http://lni.quarkkingdee.top

[R78] 交互式菜单
来源：http://gdl.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://fyw.zhongyouzk.top

[R79] 解析命令行选项
来源：http://bbw.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rax.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://hjc.kuanghao11.cn

time ./run.sh
来源：http://fgr.gzhubu.top

================================================================================
来源：http://zfy.hywenlv.cn

S. C / C++ 专题
来源：http://csx.meibo888.top

================================================================================
来源：http://gto.sufxvd.cn

[S01] C：Hello World
来源：http://aqf.hammf.cn

#include <stdio.h>
来源：http://tgm.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yfw.wangdashe.top

[S02] C：变量与格式化输出
来源：http://ckm.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://ihp.shanyushiyangtech.top

[S03] C：读入整数
来源：http://kwg.jyoumei.cn

int x; scanf("%d", &x);
来源：http://jhh.hcnkem.com

[S04] C：字符串复制
来源：http://oni.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://eso.jqgfzy.top

[S05] C：字符串长度
来源：http://tch.meibo888.top

strlen(s)
来源：http://qlk.cashguo.top

[S06] C：字符串比较
来源：http://yiy.guowangkeji.top

strcmp(a, b) == 0
来源：http://meg.bjfxy.top

[S07] C：数组遍历求和
来源：http://cgr.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zcw.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://piw.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hye.ivvv.top

[S09] C：结构体定义与初始化
来源：http://nfp.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fgu.jqgufenzy.top

[S10] C：指针与解引用
来源：http://tgl.xylfe.cn

int *p = &a;  *p = 5;
来源：http://mlg.316326.xyz

[S11] C：逐行读文件
来源：http://los.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://nen.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jye.shuidangran.top

fclose(f);
来源：http://fel.iojbl.cn

[S12] C：写文件
来源：http://gpp.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oeb.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://gxb.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vjm.chenjidiqi.icu

[S14] C：枚举
来源：http://ejc.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://uhk.fehbvm.com

[S15] C：类型转换
来源：http://qrm.gogol.net.cn

(double) a / b
来源：http://ojs.ivvv.top

[S16] C：位操作置位
来源：http://imm.yanxiufei.cn

x |= (1 << 3);
来源：http://ldy.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://cpo.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qle.ivvv.top

[S18] C：命令行参数
来源：http://lds.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://lsp.gogol.net.cn

[S19] C：快速排序
来源：http://kwh.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://pfh.dashuyun.cn

[S20] C：二分查找
来源：http://xuw.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hdm.gotoacloud.top

[S21] C：字符类别判断
来源：http://xdj.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ulw.guannengcc.top

[S22] C：字符串转数字
来源：http://lcs.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://uky.zhixingplan.top

[S23] C：随机数
来源：http://vek.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sjn.zhixingplan.top

[S24] C：获取本地时间
来源：http://jbs.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mkm.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://qgb.sweek.top

memcpy(dst, src, n);
来源：http://vgu.jinqigfzy.top

[S26] C：内存清零
来源：http://zex.xingfuxueyuan.xyz

memset(a, 0, sizeof a);
来源：http://lob.sufxvd.cn

[S27] C：定义常量
来源：http://gnw.jinqigfzy.top

const double PI = 3.14159;
来源：http://zjg.vqdsnc.cn

[S28] C：静态变量
来源：http://vac.pengpengdd.cyou

static int counter = 0;
来源：http://swx.hcnkem.com

[S29] C：变参函数
来源：http://edy.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pwe.shzxlz.cn

[S30] C：头文件保护
来源：http://oxn.ppjwa.cn


<!-- 参考信息 -->